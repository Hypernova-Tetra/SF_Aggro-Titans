## Aggro-Titans Version 1.12
- Improved a method in which to support the mod for version 1.41. (Testing and feedback needed.)
- Fixed animation for bo6190.
- An oopsie fixed with SS2's Grand Slam animation when a certain setting was set to "Vanilla (Blue Aura)"
- Moved ev1770.usm from "Parrymiss" directories to the "RifleEnd" directories.

# Aggro-Titans Version 1.11
- Monologue files adjustments.
- Fixing an audio problem in which the Italian voice line plays a line twice.
- Removed a code in Rifle01.hmm that overrides text in "sy4500_026" in other languages.
- Fixed a problem with certain voice audio of Sage, Amy, Knux, and Tails playing on the left ear in bo6140's monologue "on" setting.
- Fixed a small issue with Supreme's pillars on a QTE not glowing red energy.

# Aggro-Titans Version 1.1 (Release Feb. 01)
- Public Update Release after game update 1.42

# Aggro-Titans (Update Beta)
- Merged Monologue Add-on with Main Mod with additional options.
- Realtime Cutscene for ev5030
- Updated Final Horizons Cutscenes
- bo6110: Adjusted opening scene where The End takes over Supreme.
- bo6120 and bo6165 (SS2): Super Sonic's eyes turn blue using a certain effect before model swapping to SS2.
- bo6120 and bo6165 (Hyper): Same as the SS2 note, with the addition of adjusted effects using Cyber Sonic's particles before he turns Hyper.
- Tweaked base Supreme's cyloop animations
- Updated Winglaser v1 and v2.
- Tweaks to Supreme's Shot projectiles after destroying drones.
- Overhauled QTE files. The RNG code will choose 1 from 2 possible events instead of 3. A 3rd QTE Preset is implemented to compensate for the rearranging of files.
- Added the original "Parrymiss QTE" animation for Hyper Sonic skin mods.
- Added code file for version 1.41: To apply just modify the "mod.ini" file to match the code file for the previous game version.
- A couple of adjustments to bo4160 - I promise this is the last time.
- Added "bo6190_4k" to the GitHub Repo (in 30FPS, the 60 was too big for GitHub)
- Updated Rifle01.hmm to isolate affected lines of code after the 1.42 Update.
- Added "BossRifle_SHOT2-4_v1.42.hmm" To support the new game version.
- Added "BossRifle_SHOT2-4_v1.41.hmm" For those still on version 1.41. To apply this, open "mod.ini" and change the code file name to this file.
- Adjusted Monologue Descriptions.

# Aggro-Titans (Release Version Jan. 16)
- Public Mod Release

# Aggro Titans Pre-release Patches
Things that were done right when I thought I was done with the mod as a whole, but almost ended up missing a few things that I forgot to do, extending the original planned release date.
- R1: Further fixing QTE files so QTE inputs register properly.
- R2: Last minute tweaks to gun QTEs.
- R3: Changed cutscene bo4160.
- R4: Tweaked a certain shot for cutscene bo4110
- R5: Fixed Shoot01 in "Restored": Sonic was clipping through the first "Red Circle" QTE graphic. 
- R6: Adjusted Supreme's Drone Homing Missile to avoid a bug where the homing missiles and Supreme's counter swipe attack making Sonic unable to parry. Slight update to Supreme's idle animation.
- R7: Updated "Combat Mods" Hmm code option: Added "BossBitConfig.hmm"
- R8: Tweaked a few parameters across several scenes. Reset Supreme's idle pose back to default for the time being.
- R9: Last minute fix to Shoot01 again in "Restored" option where Sonic was clipping through another "Red Circle" QTE Graphic on the 3rd shot during the slow-motion button prompt. Fixed a scene in "Retooled" option where one of the QTE prompt types didn't match. Tweaked an animation for Supreme when parrying his counter spin attack.
- R10: Adjusted "Winglaser_v1" QTE. Added effects to a Mash QTE that was missing effects in a certain area when Supreme tried to crush Sonic with his hands. Added 4k.usm files for 4k Resolution Support for Cutscenes.
- R11: Adjusted "bo6xxx.pac". I hope it reduces lag during the SS2 transformation cutscenes.

## Aggro-Titans V0.2.2
- Adjustments to Supreme's QTE files for better pacing and to cut down on length for some.

## Aggro-Titans V0.2.1
- New Grand Slam animation for Hyper Sonic skin option when selecting "ParryMiss QTE option".
- "Zev_Parrymiss_Riflebeast.pac" adjusted to remove a detail that didn't quite make sense.

## Aggro-Titans V0.2.0
- Files reuploaded to the GitHub Repo
- Tweaks and adjustments made to Boss Health and Attack Patterns to both Rifle01 and Riflebeast
- Added Holoska's code for "AT_SHOT2" to play "Zev_Rfl_Sp02"
- Updated "Event/Scene/bo4xxx.pac" (For bo4110)

## Aggro-Titans V0.1.9
- Some adjustments to Supreme's attack speed and attack patterns.
- Adjusted Supreme's "attackHomingLaser" and "attackHandLaser" parameters.
- Adjusted "immediateActions" parameters

## Aggro-Titans V0.1.8
- Riflebeast "attackPattern" and "attackPatternAfter" slightly changed.
- Riflebeast "attackHominglaserPattern" slightly changed.
- Adjusted Winglaser_2 slightly. Fixed a problem where the QTE didn't fail immediately on the wrong button press. Second QTE prompt changed: "TheEndVariant" -> "PressPrompt".
- Other slight changes.

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
