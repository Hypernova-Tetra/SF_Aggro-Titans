## Aggro-Titans V0.1.6
- Changed animation for Riflebeast's recoil animation when parrying Claw attacks.
- Changed "slowSetting" parameters for "cyloopState" when SS2 crushes Riflebeast are adjusted. 
- se_rangers_giant04.acb file was adjusted: Sounds with the label "riflecrush" were modified to reflect changes in cyloopState listed above.
- Riflebeast's Hominglaser_Orb base speed was adjusted. 155 -> 135
- The unused "AttackHomingLaserPatterns" (Also known as "AT_HIMING") for "06, 07, 08, and 09" are implemented, though they're in a WIP state.
- Fixed cutscene "ev5040" where it loaded as a black screen.
- Fixed cutscene "ev6030" where it loaded as a black screen. Another adjustment was made to the location of Eggman and his computer console. The scene is located at the start of Ouranos Island as a temporary workaround until I figure out a way to load Chaos Island's assets to get him in his proper spot.
- ev1770 and ev5020 use the Beta Super Sonic transformation effects.
- "Boss_Bit_Param" was adjusted. 2 attacks from the drone's attack patterns have their order swapped.
- "smallbit_Laser" rotation speed adjusted. Is now the 1st drone attack that occurs when the fight starts. Before it was the 3rd attack.
- "smallbit_Homing" homingDelay and homingAccuracy slightly adjusted. Is now the 3rd attack that the drones do in order. Before it was the 1st attack.

## Aggro-Titans V0.1.5
- Optimized certain QTEs related to Shoot02 and its variants across the mod to load quicker in the fight.
- Fixed Winglaser_2 QTE's second input auto failing due to incorrect timescale parameter.
- Changed Supreme's "immediateActions" or rather what the asm file calls "counterPose" animation.
- New short QTE animation for the "Restored" option during Phase 1.
- Supreme's @attack_counter01 animation file swapped with @attack_counter04.

## Aggro-Titans V0.1.4
- Rearranged files
- Adjusted Red Circle QTE on "Zev_Blow" for Fixed Vanilla option
- Small Adjustment to the "Winglaser_2" QTE (This is still being worked on)
- Added some effects to the QTE scene from file "test_qte_sample"
- Fixed incorrect Resource Pointer from "Zev_rfl_Sp02"
- Adjusted "bo6xxx.pac" for the Hyper Sonic skin option as it was an outdated version of what I used for the Monologue mod.
- "Zev_rfl_Shoot01" had an issue with Sonic being in the wrong spot when failing parts of the QTE. So this scene was updated with new fail scenes.

## Aggro-Titans V0.1.3
- Patched Rifle01.pac
- Added and revised certain Final Horizons QTEs to support Hyper Sonic's blue outline
- Final Horizons Monologue Mod update coming soon.
- Fixed Mod.ini

## Aggro-Titans V0.1.2
- Tweaked some things.
- Fixed a soft lock from incorrect Resource Pointer parameters related to Shoot02
- Fixed a soft lock from "immediateActions" triggering "AT_Bit_Wave" in which Supreme will lock himself after spawning his drones.
  
## Aggro-Titans V0.1.1 
- Updated Combat Mod Option. Now converted to HMM code for reduced file size.

## Aggro-Titans V0.0 
-  Work In Progress
