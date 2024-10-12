## Aggro-Titans V0.1.7
- A fix for SSCyber and SSDamage model and assets not loading in the cutscene.
- Event/Scene bo6140 (Phase2) updated. Overlapping voices of Sage, Amy, Knux, and Tails are fixed.
- Adjustment to Event/Scene bo6190 (The Finale) for Hyper Sonic skins that may include slightly altered camera angle shots and added effects when Sonic going full Cyber attacks Supreme and The End.
- Reduced file size for "bo6190.usm". Eggman's scope HUD shows up in Realtime now, but only during Eggman's glasses. The scope P.O.V. still remains pre-rendered for now. I doubt I can get the POV working for Realtime.
- Event/Scene "bo4110" is slightly updated.
- Event/Scene "bo4160" is slightly updated more changes coming soon.
- Barrier HP in Extreme Mode changed: 67 -> 50

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
- Event/Scene "Zev_rfl_Sp02" in Retooled option received animation updates during the fail scene.
- Event/Scene "Zev_rfl_Shoot01" and "02 in "Retooled" Option (The extended Bitlaser01 and 02 animations) received an animation update: Extended frames during the QTE button mash phase. Different fail animation implemented depending on if the wrong button was pressed or no button was pressed, timing out the chance to win the QTE.
- Updated "Winglaser_2" animation
- Changed the "flyMoveCircleRadius" parameter so that he doesn't fly too far away and end up stuck against the Ouranos pyramid temple with no way to reach him, soft-locking he fight.
- "@attack_counter_bite_start" and "bite_dead" cam-anim files (for Supreme) are properly working now.
- Low HP phase for og Supreme's attack pattern slightly adjusted.

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
