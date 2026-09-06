# **Aggro-Titans Test** - 2026.09.06

* Current 7z Compressed Mod File Size: "1.07GB"



#### **Aggro-Titans 1.45 - Testing stuff**

* A - Trimmed out the Bool references of the Monologue options.
* B - Small code tweaks, attempting to trim the fat anywhere I can.
* C - A small code tweak to fix some possible issues cropping up.
* D - Slightly decreased Knight's arm slam speed during the Climb Phase



#### **Aggro-Titans 1.44 - Code Cleanup I guess**

* Further trimmed out unused call references across hmm files.
* Removed "Blackboard Status" element for Super Sonic, in its place using: "StatePluginBossBattle" in hmm file "SonicComboTweaks" that I forgot to update.
* Changed header title of Combat-related scripts to using "Patch" instead of using "Code".



#### **Aggro-Titans 1.43 - SS2 Aura Cutscene Fix**

* Update 3 - Code trimming on RNG functions and deleting unused reference calls in several code sections... let's hope I didn't break anything.
* Update 2 - Small script change that removed "Blackboard Status" element for Super Sonic, in its place using: "StatePluginBossBattle" to trigger functions during Boss Battles only instead of needing Super Sonic to exist.
* Update 1 - Added a new Ashrindy Script that makes Super Sonic 2's aura outline actually match the color when fighting Riflebeast. No more using DvElementAura params in Dvscenes for bo6xxx and other Riflebeast event pacs.
* Removed a few cemt assets in specific Riflebeast scenes so that Super Sonic 2's default aura is pulled from "supersonic2.pac" instead of certain event pac files.



#### **Aggro-Titans 1.42**

* Skipped to avoid confusion with the current PC/Steam version of the game.



#### **Aggro-Titans 1.41a - Battle Rush Patch**

* Fixed a problem where the Titans in Battle Rush were not using their original values.
* Fixed a problem where the Titans in Battle Rush were not using modified Medium HP values when "Boss Select Rematch" mod is active.
* Fixed an issue where the variant Super Sonic transformation scenes for Giganto weren't playing in certain intended game modes.



#### **Aggro-Titans 1.41 (Pre-Release)**

* Version bumped for final round of tests and bug searching to patch out before release, no further major development will be made.
* Fixed an error with The Final Horizons Intro of "The End" that had some caption issues and a lack of camera shaking in some parts.
* Fixed an issue where the Shield Tackle Code only functioned when Grand Slam option is set to "Unused Cinematic".
* Adjusted Combat Mod settings with the following options: "Low HP", "Medium HP", "High HP", ~~"Very High HP"~~.



#### **Aggro-Titans 1.40 (Pre-Release)**

C-10

* Updated bo2xxx to resolve an issue where Phase 2 Wyvern still had a chance of a black screen after the scene ends during the base story.
* Tweaked the Combat Mod settings. Also renamed it to "Combat Toggle".
* Chaos Polarity should now automatically toggle the bosses HP to be reduced.
* Small Tweaks to HP values and renamed "Combat Mod" name to "Titan HP" and description, then relocated the option in to "Titan Boss Setting" section.

C-09

* Updated bo4xxx.
* Fixed an error with The End's Monologue for purple aura.
* Fixed a couple of issues with Supreme.
* Buffed Wyvern Grand Slam Damage
* Updated Combat Mod option. When using Chaos Polarity, Boss HP will automatically be reduced.
* Fixed in error in where HP values may not have been reduced when Combat Mod options were on.

C-08

* Fixed a crash problem with Supreme Phase 2.
* Updated Riflebeast code file to trigger certain scenes when specific Hyper Sonic mods are active, may change aura color depending on mod.
* Overhauled ShieldTackle Removal code, will activate when certain mods and/or codes are running and updated AttackReplacers.
* Fixed a QTE in Retooled and Oops All Bitlaser that had issues.
* Updated "zev\_knight\_sonic\_damage" events.

C-07

* Code Adjustment for Phase 2 Supreme's memory address trigger.
* Updated "zev\_dragon\_finish\_00"
* Added parameter for Sonic's aura color that changes SS2's aura color when choosing the aura option.
* Updated "The End's Defeat" in Final Horizons for the blue and purple aura color option in where The End makes a desperation attack towards Sonic.

C-06

* "EventCommon" file removed due to incompatibility with the "Sock's Rio Sonic" mod.
* Moved "Eggman" texture files from "ev1770" to "bo6xxx" after discovering that apparently Eggman's textures load from this one file in Final Horizons.
* Re-added "Supreme" and "The End" texture files to only ev5040 after discovering the rest of the "World 5" scenes seem to load the assets from that one file.
* Fixed a QTE scene in Supreme's 3rd Preset

C-05

* Unused Cinematic Grand Slam code updated to trigger only for Final Horizons Story Mode due to a bug occurring when triggering the cinematic in the base game.
* Reinserted Eggman's texture files in to ev1770 after previously removing them to minimize asset reuse. There's a bit of a problem with other mods also using "EventCommon", so the bug still persists with regular Supreme for the base game's story mode with "ev5030" and "ev5040"
* Removed "zev\_end" and "zev\_end\_shooting" so that the mod manager reads these files using the vanilla files due to the previously mentioned bug in the above note.

C-04

* During the Wyvern fight, when missing a parry under certain attacks (excluding the Laser attack) in Phase 1, Wyvern may continue attack instead of chase.
* Added a new mlevel file inside the Bosscommon pac file for something specific later.
* Removed "Original" and "Sound Overhaul" audio options. Will still be available as add-ons to place above the main Aggro Titans mod.

C-03

* Updated voice files for Final Horizons Monologue
* Updated Super Sonic 2 transformation scene from ending too early.
* Small tweaks.

C-02

* Fixed an error in which the 2nd to last QTE didn't properly play during the Wyvern fight in Master King's Trial.
* Added Sonic's voices to some events.
* Small update to Final Horizons boss scenes.
* Reverted a code change to the Shield Tackle removal after the option stopped functioning.
* Updated code for Wyvern's Super Sonic transform scene in Boss Rush after the code stopped functioning.

C-01

* Available for testing.

C-00

* Reduced overall compressed mod size from 5.27GB to less than 2GB when compressed.
* Removed several usm files
* Added voice files to support bo6xxx scenes and overwrite certain cursed unused vocals found in the game.
* Added EventCommon to debloat certain scene pacs that reuse assets.
* Updated SuperSonicCyber's roar using RadicalRave's version.



Before the mod went into a downscaling phase. It was much bigger and by the end of the R22 build, the mod size was over 5GB when compressed for download.



R-22

* Went through to fix errors that may have cropped up in code files.
* Updated Supreme Cinematic Grand Slam Phase 1 camera file.

R-21

* Code tweaks again.
* Added Sonic's voice to Knight's QTEs.
* Added Sonic's voice to a small amount of Supreme's QTEs.
* Tweaked Animation for "Retooled" and "Bitlaser" QTE presets.
* Fixed an issue with Riflebeast's bo6xxx scenes in where not skipping the first SS2 power up scene causes a 3 second delay to gameplay.
* Removed toggle option for Riflebeast Darkball QTE, now a permanent feature.
* Unused Cinematic Grand Slam now has a Phase 2 animation.
* Fixed a softlock in Retooled preset due to one of the QTE files being deleted when updating.

R-20

* Another round of optimizing code files to the best of my ability.
* Animation tweaks across different scenes.
* Added unsquished Giganto intro scene. Thanks Ashrindy.
* Updated scene bo1140 for players using a no cutscene border mod to fix Super Sonic from poking out from the top of the screen.
* Small Adjustment to Wyvern's attack pattern in the "seq" section
* Added Sonic voices to Knight's QTEs.
* Fixed a crash for Knight's Phase 2 in Boss Rush.
* Added a script that hides Supreme's large drones during certain phase 2 events when played after destroying the small drones manually.
* Tweaked event animations for Supreme in "Retooled" Preset.
* Tweaked event animations for Supreme in "Bitlaser" Preset.
* Updated Monologue script to trigger when the alternate Supreme Defeat scene plays in Final Horizons instead of it triggering from loading the Ouranos Island Another Story.
* Changed a Sound file inside a custom acb.
* Deleted usm files that weren't needed.
* Fixed broken scene for Winglaser v2.

R-19

* Removed "BossCutsceneAudio.hmm" scattered its code across their respective Titan-related hmm file.
* Giganto's unused "attack\_back\_beam01\_start" for "AT\_Counter\_Sp\_03" in Boss Rush got a small tweak with Sonic's positioning.
* Separated Supreme's Intro. Default plays in Base Story, Extended plays in Final Horizons Story.
* Updated BossRifle01.hmm's "Supreme Dynamic Event" script (again).

R-18

* Added Sonic Power Boost scene that now starts and ends more quickly.
* Small animation tweaks in bo1xxx.pac
* Fixed Sonic's position after Giganto's Phase 2 event(s) end to patch a bug that occurred after implementing the Skip Cutscene feature.
* Wyvern's Missile, Psycho, and Finish QTEs now start and end more quickly.
* Custom Wyvern events in Battle Rush and Boss Rush also start and end more quickly.
* Knight's Phase 2 event now starts more quickly.
* Knight's Shieldride event now ends more quickly when succeeding the QTE prompt.
* Knight's Shieldride02 event has been tweaked slightly.
* Supreme's intro cutscene and extended intro now start and end more quickly.
* Some HMM files have been tweaked.

R-17

* Any time an event name is added or changed, "Bosscommon.pac" is updated to accommodate its updated "mlevel" file for said changes.
* "Giant01.hmm" script updated to include RNG for Giganto's knockback counter swipe attack for Boss Rush only.
* Giganto Howl attack updated. Now will play a different animation in Phase 2.
* Event files for "knight01" received an update.
* Fixed an error with an attack animation in where Knight stops moving permanently.
* Fixed an error in transformation cutscene where certain particles still persisted when the extended animation played.
* The original Final Sword QTE for Knight (zev\_knight\_atk\_sp01) has been readded for base Story "Chaos Island"
* The new Final Sword QTE that restores an unused camera pan has been moved to Boss Rush Chaos Island.
* The new Final Sword QTE's first prompt type updated from "PressPrompt" to "Red Circle".
* The new Final Sword QTE event file has been renamed (to zev\_knight\_atk\_sp03) and updated camera shot of Sonic kicking the sword.
* Certain other QTE prompts may have had their button prompts changed.
* Renamed internal files for unused Supreme Grand Slam cutscene name.
* "Rifle01.hmm" script file updated to fix up some Dynamic event cycles when performing certain actions.
* Fixed position offset errors causing the first "Winglaser" cutscene to take a while to transition back to gameplay.

R-16

* Further adjustments to some event and boss pac files.
* "Giant01.hmm" script updated to where a scene file may play a different version based on whether or not "Boss Select" mod is active and added RNG to
* "Dragon01.hmm" script updated to add a script that resets certain memory values related to Wyvern back to their default if Wyvern's object isn't loaded.
* "zev\_dragon\_sp\_missile" file updated to remove certain Near-Far settings to fix issues with Cyberspace Skybox mod rendering improperly.
* "bo3xxx.pac" file updated for scene "bo3160" to fix the same issue above.
* "BossRush.hmm" script updated to add in "Time of Day" parameters differences based on whether or not "Boss Rush Cyberspace" mod is active.
* Updated Unused Cinematic Grand Slam script to fix an error in which the scene does not trigger properly and having this option selected crashes the game when attempting to parry Riflebeast's shield tackle attack.

R-15

* Updated "bossconfig" to remove the option for Giganto's "Blue Rings", now they only show in base and Battle Rush Kronos Island while disappearing in Boss Rush (Master King Trials) Kronos.
* Further animation adjustments to the "Oops All Bitlaser" QTE preset, new animations added to certain files.

R-14

* Updated several QTE files across all 3 Presets for Supreme. Animation changes, polish, etc.
* Updated "bosscommon.pac" for updated mlevel entries.



* Fixed an issue where Wyvern's custom Phase 2 Grand Slam would crash the game.
* Updated initial "Winglaser" QTE animation.

R-13

* Fixed an issue with Giganto's Phase 2 scene not being able to be skipped in base story Kronos Island.
* Updated "bo2xxx.pac" in where the cutscene of Sonic latching on to Wyvern and being flung off before the road segment starts and ends more quickly.
* Updated Wyvern and Knight's pac files for animation tweaks.
* Resolving RNG script for Wyvern's scratch and counter attack issues.
* Resolved certain issues involving incorrect dvscene parameter values, causing sounds not to play, or the game crashes when loading the scene.
* Custom Event: "Winglaser v2" file updated with new animation.
* Updated "bo6xxx.pac"

R-12

* Giant01 HP updated: 250k -> 300k
* Dragon01 HP updated: 275k -> 325k
* Knight01 HP updated: 300k -> 350k
* Updated bo3xxx.pac to resolve transition issues.
* Updated "shieldride02\_aerial" event file.
* Rifle01 HP updated: 333k -> 385k (Base Story) / 350k -> 400k (Another Story)
* Updated Bitlaser01 and laser01 event files.
* RifleBeast HP updated: 367k -> 420k

R-11

* Fixed an error in Wyvern's Grand Slam that caused the game to crash.
* Updated "bo4xxx" and "bo6xxx"
* Updated Giganto's dynamic script files to change the defeat scene based on stage ID.
* Updated Rifle01.pac to update asm file to include new state names.
* Updated Supreme's dynamic script files to bugcheck and add RNG to Supreme's Sp02 animation.

R-10

* Updated Sound Effects for Riflebeast in "Sound Edit" to add extra Sonic grunts. (And only Sonic, no Eggman grunts.)

R-09

* Update to Riflebeast's "Final Blow" QTE files to fix an error with transitioning to either the next scene or back to gameplay when failing.
* Readded "Bossbit.hmm" for Supreme after it went missing previously.

R-08

* Adjustments to Knight's "sonic\_damage01" and custom "sonic\_damage02" event files.
* Fixed an error with one of Supreme's attack move set scripts.

R-07

* Adjustments to Script files again, merged Dynamic files with Boss hmm files.
* Adjustment to a QTE in "Vanilla Restored" preset to fix an error.

R-06

* Adjustments to bo6xxx.pac's animation files.
* Further adjustments to Supreme's QTE Preset 1 (Vanilla Restored) files.

R-05

* Several animation adjustments made to Supreme's QTE Preset files.
* Updated "bosscommon.pac" for new scene entries.
* Updated Giganto and Supreme's Dynamic script files.
* Updated Supreme's Attack Moveset scripts.

R-04

* Updated Supreme for moveset adjustments.

R-03

* Update to Riflebeast's custom Grand Slam files.
* Updated Riflebeast's pac file.

R-02

* Readded several mod files to fix issues.
* Clean-up for file size optimization.

R-01

* Several small tweaks.
* Added missing .usm files.

R-00

* Revamped Monologue option, now runs on HMM code with new scene files based on selected option combinations.
* Overhauled HMM scripts
* Updated Riflebeast QTE files for "Final Blow" and "Parry Miss"
* Updated Riflebeast Grand Slam Files.
* Updated "bo6xxx" file.
* Additional changes to Giganto and Supreme.
* "Bosscommon.pac" updated to include new scene entries for Monologue option.



*Test Version 1.39*

R-02

* Another round of changes
* Readded "zev\_sp\_riflebeast" for skin mods using "SuperSonicDamage" and "SuperSonicCyber" assets.

R-01

* Updated Version String
* Updated "mod\_files.txt"

R-00

* HMM Script changes to Dynamic Event files for the Titans.
* Removed unneeded usm files.
* Changes to Giganto, Supreme, bo6xxx, Bitlaser01, and other files.
* Changes to Knight's formerly unused "ShieldRide02\_aerial"
* Changes to Knight's bo3xxx file.
* Changes to Supreme's "zev\_rfl\_sp02" file.
* Changes to audio files for Knight and Supreme.



*Test Version 1.38*

* Supreme's QTE dynamic script rewritten by GordonRamsy (Huge Thanks)
* Some adjustments to "Dynamic" files for the other Titans.



*Test Version 1.37*

Giant01 (Giganto)

* Updated Giganto's ImmediateActions between base game and Master King Trials
* Changes to "AT\_HOWL" in where the attack itself will now play sound effects.
* Changes to "AT\_COUNTER\_SP\_01" in where '@attack\_counter\_bite\_end.cam-anim' is now more accurate to the Frontiers 2021 Beta leak footage.
* Implemented a leftover action for "AT\_COUNTER\_SP\_03" in Master King's Trial for Giganto to play a previously unused laser attack animation.
* Giganto Finale option adjusted.
* "Tru-Blu Giganto Finale" moved to Master King's Trial.
* "Tru-Blu Giganto Super Sonic Transformation" added for Master King's Trial.
* "BOI's animation" for Super Sonic added and will play in Main story Kronos.
* "Vanilla" Super Sonic scene will play in Battle Rush only.
* Adjustments made to GiantDynamics.hmm



Dragon01 (Wyvern)

* "BOI's animation" for Super Sonic added and will play Master King's Trial.
* "Vanilla" Super Sonic scene will play in Battle Rush and Main Story.
* "Dragon\_Finish\_00" moved to Master King's Trial.



Knight01 (Knight)

* "BOI's animation" for Super Sonic added and will play Master King's Trial.
* "Vanilla" Super Sonic scene will play in Battle Rush and Main Story.



Rifle01 (Supreme)

* Changes to "AT\_SP02" in where the starting Mega Laser attack animation has been updated to keep its uniqueness.
* Small changes to some of Supreme's "giantPhase" actions.
* Updated "WingLaser" QTE files. They should hopefully take less time for the event to start.
* Winglaser's config option is now in code form rather than folders.
* Winglaser's config now has an "Off" option to play a different event instead, but will only occur when Supreme reaches low health.
* New "Bitlaser03" scene implemented for first encounter.
* RifleBeast Changes
* In bo6xxx.pac: Reduced loading time for Riflebeast Cutscenes bo6110, bo6125, bo6130, bo6140, bo6150, bo6160, bo6190 and its variants for the FH Monologue option.



*Test Version 1.36*

* Further tweaks to Super Sonic 2's transformation for the "Edited" Animation type: Now references the Final Horizons Trailer camera panning when first transforming.



*Test Version 1.35*

* Overhauled Monologue entries, less folders, more streamlined.
* Some tweaks in bo6120, bo6165, and bo6190.
* Tweaked a combo-move for Sonic only when Supreme's "Unuse Cinematic Event" is active during Supreme's fight.



*Test Version 1.34*

* Fixed a typo in one of the config values
* Update Sonic 0 Ring Cutscene for Phase 2 in Supreme's fight.
* Updated bo1xxx.pac to fix some errors



*Test Version 1.33*

* Updated code to have "AT\_Tackle" be automatically disabled when "Unused Grand Slam Event" option is selected for Supreme.
* Added Tru-Blu animation for Super Sonic Transformation for Master King's Trial only.
* Added Tru-Blu Giganto Defeat as a 4th Option in Giganto Finale section.
* Updated scene file: "zev\_rfl\_wing.pac"



*Test Version 1.32*

* BossEvent.hmm and BossTitanFinish.hmm files removed.
* Added "Boss(Name)Dynamics" hmm files for their respective Titan bosses and the code for "TitanFinish" is moved to the Dynamics hmm files based on the respective Titan.



*Test Version 1.31*

* Updated "bo3xxx.pac" Super Sonic now shows up when the Super Sonic transformation scene transitions to the fight.
* Updated Grand Slam scene file for Riflebeast in name only for Phase 1 to avoid conflicts with Sonic skin mods.



#### **Aggro-Titans 1.30**

* Bumped to version 1.3 for release.



*Test Version 1.26*

* Updated "bo1xxx.pac" includes a new Phase 2 scene exclusive to Master King's Trial courtesy of Tru-blu.
* Added a toggle option for Sonic's Animation Speed Changes
* Very small update to Supreme's subphases in Phase 1.
* Tweaked .hmm code files to iron out potential issues with performance problems.
* Tweaked BossEvent.hmm, BossRifle01.hmm, and BossRiflebeast.hmm by reimplementing certain changes based off version 1.25b and improved them with the newer changes.
* Improved Unused Grand Slam Event animation for Supreme.
* Changed Memory Address of Giganto's Beta Defeat cutscene in the mod's coding to not inflict with an unused memory address with the game.
* Lowered the HP of the Titans when using non-modded Max Stat Sonic.
* Added a toggle option to choose between Default Texture and MatiosDX's Fitting Textures mod.
* A variant of Wyvern's Psycho QTE was added that restores an unused shot. Some tweaks to Wyvern were made.
* Fixed a sound sync error in a scene.
* A slight tweak to the custom scene of Supreme's defeat.
* Supreme's Intro Cutscene config option has under-the-hood tweaks done.
* Giganto's blue rings have a toggle option.
* Wyvern Counter Laser animation tweaked. The unused version now plays at Phase 2 on either side of Wyvern



*Test Version 1.25*

* Final touches in certain areas.
* Updated Supreme's attacks.
* Phase 1 QTEs are more dynamic.
* Fixed a softlock issue.
* Fixed a crash issue with Riflebeast Tackle Attack somehow caused by activating the unused Grand Slam event for regular Supreme.
* The Ouranos Pyramid's Chaos Emerald pillar effect now disappears when in base game's Supreme fight and will respawn when reloading the save file. (Why does a mod need to address this problem)
* Sonic's 0 Ring Cutscenes (bo1180, bo2180, bo3180, and bo4180) have a Phase 2 version added.
* Fixed an issue with Riflebeast's cable asset not using the correct animation during the Darkball QTE.
* Fixed the issue in where Riflebeast's Material and UV animations didn't play properly in certain cutscenes.
* Config tweaks.
* No more confliction with other mods using "master.levels" file.
* Restored unused Cyloop Counter animation for Giganto.
* Code Tweak for Wyvern's Phase 2 cutscene when the "Skip" option is active. Reverted to Lua.Call functions to fix a lingering issue with Sonic being respawned in the wrong spot after the cutscene ends.
* Textures for Wyvern and Knight have been changed, using the "Fitting Titan Re-textures Mod" by MatiosDX. Wyvern reflects the purple-tier enemies while Knight now reflects the red-tier enemies.
* Fixed a cutscene error and did some other tweaks across different parts of the mod.
* Supreme QTE adjustments. Both Winglasers now show up in the same battle.



*Test Version 1.24*

* Slight tweaks to Rifle01 attack patterns
* Tweaked "BossRifle01.hmm" to reflect the changed attack patterns across Phase 1's immediate Actions for Final Horizon.
* Tweaked "BossEvent.hmm" so it uses less code for Supreme's Dynamic Events. No longer separated between versions of Ouranos Island.
* Removed a Lua.Call for "PlayingDiEvent" across multiple sections of code in favor of new code that achieves the same function.
* Added "Sound Overhaul" as a 3rd option to the Titan Audio settings.
* Updated code that removes Riflebeast's Tackle Attack courtesy of thej01.
* Updated Unused Grand Slam Cinematic code. (Still need to investigate an issue involving this code.)
* Reworked "Bitlaser01" and "Bitlaser02" for the "Retooled" QTE option, didn't like the old one too much.
* Very small tweaks to Wyvern, Knight, and Supreme's QTE files.



*Test Version 1.23*

* New option added in Riflebeast's config setting. (Darkball QTE) (Currently Experimental)
* Adjusted Cutscene bo6190 to fix an error.
* Fixed an oversight with code "Dynamic\_Sp02" in BossRifle01.hmm
* Fixed a 1 frame camera error in Cutscene bo4140.
* Adjusted "Counter\_Attack" RNG code for Giganto and Supreme
* Optimized .hmm code files for "Rifle01.hmm" and "BossRifleBeast.hmm" to fix instability problems in Final Horizons Ouranos Island.
(Did I finally fix the Crash Problem on Final Horizons Ouranos Island?)
* Very small barely noticeable tweaks made to 3 animation files for Supreme.
* Fixed a Battle Rush QTE error in which a Phase 1 QTE appeared in Phase 2.
* Adjustments to Knight.
* Alternate Sword QTE added for Battle Rush.



*Test Version 1.22*

* Attempting to adjust and fix random crash issues with Riflebeast (turns out it's a memory leak problem.)
* New Sword RNG attacks for Knight in Phase 1.
* New Sword Counter Attack for Knight in Phase 2
* Adjusted scene: "zev\_parrymiss\_riflebs03"



*Test Version 1.21*

* Fixed the Edited "parrymiss" QTE having missing sounds when Riflebeast strikes Sonic to start the QTE.
* Fixed the Edited "Final Blow" Riflebeast QTE having the wrong sound effects that used different names.
* Updated "master.levels" in the Hedgehog folder.
* Small update to bo6125 and bo6190.
* Updated bo6190.usms.
* Another adjustment Supreme's Event files to implement gradual changes to the Bitlaser Event Slot for Phase 1 and 2. BIG shoutout to Holoska for this implementation.
* Adjusted Address Memory code scripts for Unused Supreme Grand Slam Event.
* Adjusted audio for Knight's Grand Slam Event Scene.
* Parrymiss QTE options updated, the "Edited" version is now a Phase 2 QTE during the fight.
* New QTE added, reuses "bo6160" for a new QTE in-place of Parrymiss for Phase 2 of The End's fight only after the player gets hit with the homing laser attack to start the cutscene of Sonic surviving The End's Dark Ball.
* Adjustments made to Wyvern's boss file and hmm code file.
* Several adjustments have been made across other hmm code files.
* Fixed Supreme from disappearing in Phase 2.
* "extra\_sound" directory added.
* Wyvern Phase 2 Grand Slam added.
* File and Code Adjustments made.



#### **Aggro-Titans 1.20**

* Supreme's scratch attacks are slightly faster.
* Supreme's Bit Drone projectiles have been retextured.
* Supreme's Bit Drone attacks are slightly more aggressive.
* Rearranged Supreme's QTE files.
* Updated animations to Supreme's QTEs and defeat cutscene.
* Changes to Supreme's Wing Laser QTE were made and is exclusive to Final Horizons Supreme fight.
* Converted Supreme's Grand Slam into the unused cutscene. (Doesn't do damage, but will give rings while "Combat Mods" is active.
* Final Horizons Cutscenes updated.
* bo6120: Added new effects from Sonic's stat boost cutscenes. Will be red when using the "Edited" option. Will be Red/Blue for the "Hyper\_Blue Aura" options. The Power Boost eye effect has been repositioned properly so that it better overlaps the eyes better. (Can't change their color for now though.)
* bo6165: The "blue-eye" effect for SS2 has been properly positioned to overlap the eyes.
* Giganto, Wyvern, and Knight added to the mod.
* Giganto received adjustments to restore unused attacks and have his attacks more aggressive.
* New animation for Giganto's defeat using leftover files possibly from the beta have been added.
* Giganto's "bo1xxx.pac" updated to have additional content. (Making this mod have higher priority over other mods using this file.)
* Adjusted Giganto's Sp01 attack. Giganto's "Counter\_Bite\_Start" pose was updated to utilize an unused animation file. "Counter\_Bite\_Loop" camera animation from the beta has been implemented.
* Added a small extra animation for the start of Giganto's Sp02 attack that originally wasn't there before.
* bo1120: Super Sonic's transformation cutscene is updated to include an unused animation for Super Sonic and a almost seamless transition to the fight.
* bo1150: Added as a variant for Giganto's defeat. This is primarily based off of leftover beta files left in the game.
* bo1170: Added as another variant for Giganto's defeat. This is a mixed version of the Beta and the Final's animations.
* bo1180: Added the unused "Zero Ring Warning" sound effect. Other than that, mostly remains unchanged.
* Wyvern's attack patterns are slightly adjusted.
* Wyvern's scratch attack animation and animation speed are slightly adjusted.
* Added more chances to attack Wyvern after failing to parry his attacks.
* Wyvern's "bo2xxx.pac" updated to have additional content.
* bo2120: Updated Super Sonic's transformation cutscene.
* bo2180: New animation was added when Sonic loses his rings.
* Phase 2 "Chase" after the transition cutscene has been moved.
* Parry slow effect adjusted.
* Wyvern will counter attack more times before the laser.
* New animation added in Wyvern's Missile QTE when failing.
* Wyvern's Events may change briefly after Phase 2 in the Master King's trials.
* Restored Unused "Counter\_Laser" animation if you're on Wyvern's LEFT side.
* Unused Beta-inspired Finale implemented and configurable.
* Knight's climb phase updated to have the hand slam go by a bit faster
* Knight's sword slash animations are adjusted a little. (Still in a WIP. I'll adjust them based on feedback.)
* Knight's Battle Start animation was moved in to cutscene bo3120, making the fight start sooner instead of waiting for Knight to pull his sword out.
* Knight's QTEs adjusted:
* "shieldride01": Remains unchanged for the most part in terms of its animation, but the QTE prompt is a bit faster now.
* "shieldride01\_short": Slight animation change in how Knight tosses the shield, QTE button changed, and ends early when winning the QTE.
* "shieldride02": New segment added so it's not a complete copy of "shieldride01\_short" using a new file.
* Knight's "bo3xxx.pac" updated to have additional content.
* bo3120: Updated to include Knight's Battle Start animation where he pulls the sword out.
* bo3180: New animation was added when Sonic loses his rings.
* Knight's "Grand Slam" for Phase 2 may instead play a QTE at a random chance.
* Cutscene: "zev\_knight\_sonic\_sp01\_phase2" is updated. Cylinders weren't protruding as they should be, and Sonic will punch the Titan as the final attack instead of kicking him down.
* Knight's "Sword QTE" was updated to reflect his Phase 2 appearance and adds a cut segment where the camera will pan to Sonic preparing to catch the sword.
* Master King Trials have been adjusted to reflect the new changes.
* All the above changes to Giganto, Wyvern, and Knight are automatically reflected in the MK trials since they use the same pac files.
* Rings will be granted between fights in Master King Trials.
* Added a condition to earn rings from parrying while ring count is low during the Wyvern fight.
* Giganto and Knight can also grant rings via cylooping them and Grand Slam.
* Time of Day is adjusted.
* Experimental changes to Phase 2 cutscene for Giganto, Wyvern, Knight, and base Supreme to be skippable. (Sonic's position might be affected)



#### **Aggro-Titans 1.12**

* Improved a method in which to support the mod for version 1.41.
* Fixed animation for bo6190.
* An oopsie fixed with SS2's Grand Slam animation when a certain setting was set to "Vanilla (Blue Aura)"
* Moved ev1770.usm from "Parrymiss" directories to the "RifleEnd" directories.



#### **Aggro-Titans 1.11**

* Monologue files adjustments.
* Fixing an audio problem in which the Italian voice line plays a line twice.
* Removed a code in Rifle01.hmm that overrides text in "sy4500\_026" in other languages.
* Fixed a problem with certain voice audio of Sage, Amy, Knux, and Tails playing on the left ear in bo6140's monologue "on" setting.
* Fixed a small issue with Supreme's pillars on a QTE not glowing red energy.



#### **Aggro-Titans 1.10**

* Public Update Release after game update 1.42

(Update Beta)

* Merged Monologue Add-on with Main Mod with additional options.
* Realtime Cutscene for ev5030
* Updated Final Horizons Cutscenes
* bo6110: Adjusted opening scene where The End takes over Supreme.
* bo6120 and bo6165 (SS2): Super Sonic's eyes turn blue using a certain effect before model swapping to SS2.
* bo6120 and bo6165 (Hyper): Same as the SS2 note, with the addition of adjusted effects using Cyber Sonic's particles before he turns Hyper.
* Tweaked base Supreme's cyloop animations
* Updated Winglaser v1 and v2.
* Tweaks to Supreme's Shot projectiles after destroying drones.
* Overhauled QTE files. The RNG code will choose 1 from 2 possible events instead of 3. A 3rd QTE Preset is implemented to compensate for the rearranging of files.
* Added the original "Parrymiss QTE" animation for Hyper Sonic skin mods.
* Added code file for version 1.41: To apply just modify the "mod.ini" file to match the code file for the previous game version.
* A couple of adjustments to bo4160 - I promise this is the last time.
* Added "bo6190\_4k" to the GitHub Repo (in 30FPS, the 60 was too big for GitHub)
* Updated Rifle01.hmm to isolate affected lines of code after the 1.42 Update.
* Added "BossRifle\_SHOT2-4\_v1.42.hmm" To support the new game version.
* Added "BossRifle\_SHOT2-4\_v1.41.hmm" For those still on version 1.41. To apply this, open "mod.ini" and change the code file name to this file.
* Adjusted Monologue Descriptions.



#### **Aggro-Titans (Release Version Jan. 16)**

* Public Mod Release



#### **Aggro-Titans Pre-Release**

(Things that were done right when I thought I was done with the mod as a whole, but almost ended up missing a few things that I forgot to do, extending the original planned release date.)

* R11: Adjusted "bo6xxx.pac". I hope it reduces lag during the SS2 transformation cutscenes.
* R10: Adjusted "Winglaser\_v1" QTE. Added effects to a Mash QTE that was missing effects in a certain area when Supreme tried to crush Sonic with his hands. Added 4k.usm files for 4k Resolution Support for Cutscenes.
* R9: Last minute fix to Shoot01 again in "Restored" option where Sonic was clipping through another "Red Circle" QTE Graphic on the 3rd shot during the slow-motion button prompt. Fixed a scene in "Retooled" option where one of the QTE prompt types didn't match. Tweaked an animation for Supreme when parrying his counter spin attack.
* R8: Tweaked a few parameters across several scenes. Reset Supreme's idle pose back to default for the time being.
* R7: Updated "Combat Mods" Hmm code option: Added "BossBitConfig.hmm"
* R6: Adjusted Supreme's Drone Homing Missile to avoid a bug where the homing missiles and Supreme's counter swipe attack making Sonic unable to parry. Slight update to Supreme's idle animation.
* R5: Fixed Shoot01 in "Restored": Sonic was clipping through the first "Red Circle" QTE graphic.
* R4: Tweaked a certain shot for cutscene bo4110
* R3: Changed cutscene bo4160.
* R2: Last minute tweaks to gun QTEs.
* R1: Further fixing QTE files so QTE inputs register properly.



V0.22

* Adjustments to Supreme's QTE files for better pacing and to cut down on length for some.

V0.21

* New Grand Slam animation for Hyper Sonic skin option when selecting "ParryMiss QTE option".
* "Zev\_Parrymiss\_Riflebeast.pac" adjusted to remove a detail that didn't quite make sense.

V0.20

* Files reuploaded to the GitHub Repo
* Tweaks and adjustments made to Boss Health and Attack Patterns to both Rifle01 and Riflebeast
* Added Holoska's code for "AT\_SHOT2" to play "Zev\_Rfl\_Sp02"
* Updated "Event/Scene/bo4xxx.pac" (For bo4110)

V0.19

* Some adjustments to Supreme's attack speed and attack patterns.
* Adjusted Supreme's "attackHomingLaser" and "attackHandLaser" parameters.
* Adjusted "immediateActions" parameters

V0.18

* Riflebeast "attackPattern" and "attackPatternAfter" slightly changed.
* Riflebeast "attackHominglaserPattern" slightly changed.
* Adjusted Winglaser\_2 slightly. Fixed a problem where the QTE didn't fail immediately on the wrong button press. Second QTE prompt changed: "TheEndVariant" -> "PressPrompt".
* Other slight changes.

V0.17

* A fix for SSCyber and SSDamage model and assets not loading in the cutscene.
* Event/Scene bo6140 (Phase2) updated. Overlapping voices of Sage, Amy, Knux, and Tails are fixed.
* Adjustment to Event/Scene bo6190 (The Finale) for Hyper Sonic skins that may include slightly altered camera angle shots and added effects when Sonic going full Cyber attacks Supreme and The End.
* Reduced file size for "bo6190.usm". Eggman's scope HUD shows up in Realtime now, but only during Eggman's glasses. The scope P.O.V. still remains pre-rendered for now. I doubt I can get the POV working for Realtime.
* Event/Scene "bo4110" is slightly updated.
* Event/Scene "bo4160" is slightly updated more changes coming soon.
* Barrier HP in Extreme Mode changed: 67 -> 50

V0.16

* Changed animation for Riflebeast's recoil animation when parrying Claw attacks.
* Changed "slowSetting" parameters for "cyloopState" when SS2 crushes Riflebeast are adjusted.
* se\_rangers\_giant04.acb file was adjusted: Sounds with the label "riflecrush" were modified to reflect changes in cyloopState listed above.
* Riflebeast's Hominglaser\_Orb base speed was adjusted. 155 -> 135
* The unused "AttackHomingLaserPatterns" (Also known as "AT\_HIMING") for "06, 07, 08, and 09" are implemented, though they're in a WIP state.
* Fixed cutscene "ev5040" where it loaded as a black screen.
* Fixed cutscene "ev6030" where it loaded as a black screen. Another adjustment was made to the location of Eggman and his computer console. The scene is located at the start of Ouranos Island as a temporary workaround until I figure out a way to load Chaos Island's assets to get him in his proper spot.
* ev1770 and ev5020 use the Beta Super Sonic transformation effects.
* "Boss\_Bit\_Param" was adjusted. 2 attacks from the drone's attack patterns have their order swapped.
* "smallbit\_Laser" rotation speed adjusted. Is now the 1st drone attack that occurs when the fight starts. Before it was the 3rd attack.
* "smallbit\_Homing" homingDelay and homingAccuracy slightly adjusted. Is now the 3rd attack that the drones do in order. Before it was the 1st attack.
* Event/Scene "Zev\_rfl\_Sp02" in Retooled option received animation updates during the fail scene.
* Event/Scene "Zev\_rfl\_Shoot01" and "02 in "Retooled" Option (The extended Bitlaser01 and 02 animations) received an animation update: Extended frames during the QTE button mash phase. Different fail animation implemented depending on if the wrong button was pressed or no button was pressed, timing out the chance to win the QTE.
* Updated "Winglaser\_2" animation
* Changed the "flyMoveCircleRadius" parameter so that he doesn't fly too far away and end up stuck against the Ouranos pyramid temple with no way to reach him, soft-locking he fight.
* "@attack\_counter\_bite\_start" and "bite\_dead" cam-anim files (for Supreme) are properly working now.
* Low HP phase for og Supreme's attack pattern slightly adjusted.

V0.15

* Optimized certain QTEs related to Shoot02 and its variants across the mod to load quicker in the fight.
* Fixed Winglaser\_2 QTE's second input auto failing due to incorrect timescale parameter.
* Changed Supreme's "immediateActions" or rather what the asm file calls "counterPose" animation.
* New short QTE animation for the "Restored" option during Phase 1.
* Supreme's @attack\_counter01 animation file swapped with @attack\_counter04.

V0.14

* Rearranged files
* Adjusted Red Circle QTE on "Zev\_Blow" for Fixed Vanilla option
* Small Adjustment to the "Winglaser\_2" QTE (This is still being worked on)
* Added some effects to the QTE scene from file "test\_qte\_sample"
* Fixed incorrect Resource Pointer from "Zev\_rfl\_Sp02"
* Adjusted "bo6xxx.pac" for the Hyper Sonic skin option as it was an outdated version of what I used for the Monologue mod.
* "Zev\_rfl\_Shoot01" had an issue with Sonic being in the wrong spot when failing parts of the QTE. So this scene was updated with new fail scenes.

V0.13

* Patched Rifle01.pac
* Added and revised certain Final Horizons QTEs to support Hyper Sonic's blue outline
* Final Horizons Monologue Mod update coming soon.
* Fixed Mod.ini

V0.12

* Tweaked some things.
* Fixed a soft lock from incorrect Resource Pointer parameters related to Shoot02
* Fixed a soft lock from "immediateActions" triggering "AT\_Bit\_Wave" in which Supreme will lock himself after spawning his drones.

V0.11

* Updated Combat Mod Option. Now converted to HMM code for reduced file size.

V0.10

Work In Progress



#### **Version 0 Demo**

***Rifle01 - Supreme***

* Increased HP
* Slightly faster attacks
* A complete overhaul to his attack patterns
* Multiple attack patterns at different HP thresholds.
* All possible unused attacks from Supreme are restored.
* All possible unused attacks by Supreme's drones have been restored.
* Every now-and-then Supreme will interrupt the player to perform a counterattack. (This is known as "immediateActions" in the rfl file)
* Added Wings for Phase 2 (Thank the heavens and thank everyone that helped me through getting this to work.)
* An overhaul to the boss's sound effects for certain attacks, certain cutscene sounds were moved to .usm files to make room for new sounds.
* Supreme's "@attack\_counter" (Which is known as AT\_Counterblow in the rfl) can randomly play different animations. (Thanks to Holoska for this.) Due to this change, it also affects Giganto as they share the exact same animation file name.
* Supreme's QTEs have a random selection of events that trigger when Supreme's drones are destroyed at certain points of the fight. (Thanks to Holoska for this too.)
* Certain animation files of Supreme in the base fight were tweaked just so that it's not a complete copy-paste of Giganto.
* "Zev\_Rfl\_Bitlaser" is now a QTE.
* All unused QTEs restored with tweaks to have it be somewhat unique.
* New QTEs in a "Retooled" option for the mod that may feature new animations but definitely uses some unused animation files that were hiding in the files.
* A new QTE during Phase 2 only that utilizes his wings, even though it's just him shooting a bigger laser than "@attack\_CounterSp02".
* Extended Intro and Revised Outro scene.
* Certain miscellaneous details have been fixed.
* Missing effects from Supreme's "@attack\_counterSp02" and "smallBit\_laser" have been restored, thanks again Holoska.

Things to do:

* Fix the error of Supreme's Cylinders. The middle one on his shoulders don't show during gameplay.
* Continue checking for bugs and issues.

***Riflebeast - The End***

* Increased HP
* Increased cable HP. (Cyloop may be recommended to break the cable now.)
* Alternate attacks between his Hominglaser Orbs and Triple Claw attack.
* Slightly changed his attack patterns.
* Possibly fixed the issue with trees obscuring the player's view, but this may come with a new issue of obscuring the view of the Homing orbs attacking Sonic. This still needs to be further tested.
* Slightly increased Hominglaser\_Orbs' attack speed.
* Fixed a mis-render. "Super Sonic 2" should now be seen instead of regular Super Sonic when the Phase 2 cutscene plays. Don't know how this ended up happening.
* Fixed the Realtime Cutscene's Mod for Cutscene Bo6190 where Eggman's HUD scope isn't shown.
* Fixed a mis-render of SS2's aura not visible when performing the QTE of escaping Supreme's grip, after failing the initial Final Blow QTE
* Fixed another mis-render of SS2 himself not being visible when escaping Supreme's grip.
* There's an option for said "Final Blow QTE" in the mod to either use the original version, or an edited version to where the latter half of the Final Blow QTE isn't reusing the "Parrymiss" QTE. The QTE prompts are also changed in the initial parts of the QTE.
* The End Monologue from base game is implemented followed by a restoration of unused captions related to said monologue. This is a togglable option.
* Added a slow-mo effect when parrying Supreme's "Triple Claw" attack. I also slightly modified beast's normally unseen animation where his hand recoils after the attack is parried.
* Slightly modified SS2's transformations in both bo6120 and bo6165. This may need further tweaking for performance's sake.
* Originally in Phase 1, Supreme would enter a stunned state when his health reaches 50%. This has been changed so that he gets stunned when his health reaches 0.

