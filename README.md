# Aggro-Titans

Creator: 
- Hypernova

Contributors:
- Adel
- Holoska
- Ashrindy
- Elise
- DoomGuyRi/NuggetHead
- TheLukeSpark
- DJ Scout
- TheMoe
- Dawghouse294
- ButterDee
- BatmanSonic
- Stis
- Blitz
- ik-01
- Skrud
- The Duck Dealer
- GordinRamsay
- Nowasu

Special Thanks to everyone.

Starting out as an ambitious mod for only Supreme to restore and overhaul the supplied content we were given throughout the endgame's final moments. 

After several members of the modding community went under the hood and discovered plentiful unused things that Supreme was unfortunately never given the chance to show off, this mod aims to give full functionality of what was left behind, along with some creative freedom to shake up the fight so that Supreme's animations aren't a complete 1-to-1 with Giganto. 

There was a lot done with this mod so bear with me. There are certain things I cannot fix. This mod will be updated later for the other 3 Titans to have a spotlight of some content restoration.

--------------------------------------------------------------------------------------------------------------------------------------------------
Firstly, this mod's Titan health is adjusted to fit a max attack level vanilla combat Super Sonic. There is a "Combat Mod" option that uses HMM code to lower the boss health to fit the often-nerfed damage output that certain combat mods bring.

--------------------------------------------------------------------------------------------------------------------------------------------------
Titan: Supreme
The attacks that have been restored: (names referenced from "boss_rifle.rfl")
- AT_Laser:
(A technical unused attack that Supreme uses that makes him fire multiple shots from his mouth. While the description is normally seen after destroying his drones, this version just has him start blasting away. Oddities of this attack when implemented feature Supreme having a chance to become idle for a long time if moved too far from his line of sight. To remedy this, cyloop him or force him to counterattack by attacking him when his drones are still up. If this doesn't happen to you, you should be fine.

- AT_Sp01:
Giganto's Clap-Bite QTE. Works as expected for the most part. Including a unique camera animation normally unseen when the titan goes for a bite. The camera was not meant to be stationary when Supreme (or Giganto for that fact) when either of the Titans bite Sonic. I found an oddity to the attack to where, if implemented in a certain way that isn't in Supreme's "immediateActions" parameter, Supreme may force the Bitlaser event if the player parries the clap but doesn't follow up with a Grand Slam or Cyloop in time. This is probably due to how the BitLaser is triggered by using the "Sp01" attack. 

- AT_Sp02:
Giganto's Mega Laser QTE. Not much to explain here. It's just the titan firing a giant laser from the mouth for Sonic to repel back. Oddities of this attack include a couple of effects not showing up properly. "Laser01_Guard" is tied to Super Sonic. Has been fixed by placing said cemt effects into Rifle01.pac as they reuse Giant01.pac's cemt files.  "Laser01_Omen" wasn't properly shown due to some shenanigan with Supreme's other files. This has been properly fixed up as well and will show up. A unique animation for this attack utilizes an unused animation that both Supreme and Giganto share (File: "@attack_back_beam01"). Will only be implemented for Supreme in this mod.

- AT_Counterblow:
Giganto's right-handed swipe attack. It comes in 3 different animation files as: "@attack_counter01", "@attack_counter02", and "@attack_counter03". These animations go unused for Supreme. When implemented, it will only use "counter01" as a default. Thanks to Holoska, the counterattack animations will play at random when "Counterblow" is triggered.

- AT_HomingLaser:
This attack has Supreme standing (or floating if triggered in Phase 2) in one spot and will proceed to fire homing shot laser projectiles out of the shoulder holes of his backpack. Parrying the shots destroys the projectiles and will not send them back to Supreme for some reason. I also cannot find out what controls their firing speed. I'm not sure what this attack was meant for. Perhaps this attack was reworked into the Final Horizons Supreme fight?

- AT_HomingLaser_Fly:
This attack has Supreme actively flying in a set path around the arena while firing homing shot projectiles out of the shoulder holes of his backpack at a slightly faster speed. Parrying the shots won't do anything here as well except de-spawn the projectiles. Unsure of what this attack was meant for.

Supreme's small drones have also been tweaked. 2 unused attacks were implemented that gave the turrets more firepower.

- smallBitPatternDatas_bulletType (Laser):
Discovered by DatSquishyFellow. This attack has Supreme's surrounding turrets fire a laser beam to enclose the player in a specific area for a short amount of time. However, what was missing was the lasers themselves. For the longest time the beam effect wasn't able to be shown. There's also a problem with this attack in which the open space that allow the player to freely approach Supreme is blocked by an invisible object that sends Sonic flying. If someone can help me with a fix for this... please contact me. I could really use the help with this. At some point it was found out by Holoska that the files coded into the game for the beam effect are reused Giganto files, who would have guessed. By placing certain cemt files of the laser beam from Giant01.pac into Rifle01.pac the laser beams have been restored.

- smallBitPatternDatas_bulletType (Homing):
Discovered by giant01poofy. This attack turns the turrets upward, facing the sky as black missiles that cannot be parried will fire out and begin tracking the player. The only way to actually block these missiles is if Sonic is in mid-parry animation from parrying another attack entirely as the missiles hit him. 

QTES Restored and overhauled
Found inside "boss_rifle.rfl" are 4 "ActionType" moves that trigger Supreme's QTEs. "AT_SHOT1", "AT_SHOT2", "AT_SHOT3", and "AT_SHOT4" were meant to play 4 different Event Scene files located in the Frontiers "event/scene" directory, but this action was not fully finished. While AT_SHOT1 and 2 both trigger the gun QTE where Supreme fires a yellow bullet... SHOT3 and 4, when implemented in the boss's file and no additional changes are made, have a problem that soft locks the fight. This is because the game's executable file has a name error of the scene name that the game tries to load but cannot find due to the mismatched name. This mod fixes that issue in a couple of ways thanks to Holoska's help.

Supreme's Sp01 and Sp02 attacks have an event/scene variant to them that suggests perhaps the "Clap-Bite" and "Mega Laser" events were going to perhaps play out a bit differently but sadly aren't finished. This mod completely restores them and adds new elements to the events so that they aren't a complete copy of Giganto.
--------------------------------------------------------------------------------------------------------------------------------------------------
This mod contains multiple QTE slots across 2 different option types that not only restore the unfinished events in the game but are packed with new animations and new QTEs to add more spice to the boss.

--------------------------------------------------------------------------------------------------------------------------------------------------
* Ouranos Island Supreme Type Option: "Restored"*
- "test_sage_move.pac" (Formerly Zev_rfl_sp01: "Clap-Bite" The original unfinished scene):  
When failing the initial "Clap" QTE, Supreme will bite Sonic using an unused alternate bite animation that Giganto and Supreme never use. It plays out the same as needing to mash the prompted button to escape. However, if you fail this part, Supreme will not hesitate to shoot Sonic out of his mouth by firing a laser beam. 

( Why this event was moved out of the original slot and into a different one will be explained later.)

- "Zev_rfl_Sp02.pac" (Mega Laser): 
Plays out similar to the attack Giganto uses. Except with some changes compared to Giganto's version, and Supreme's unused AT_Sp02 attack. Supreme's pillars are exposed to indicate the event is meant to be seen in Phase 2. The scene plays out similarly to its unused version, with the change that the camera angle for Sonic holding back the laser is much different. The QTE fail scene only adds in effects that were not present before. Passing the QTE however, Sonic will send the laser attack back to Supreme's face. The only problem with this that Supreme won't have his HP damaged. Supreme is missing parameters in his .rfl file that trigger damage values in comparison to the other titans. If someone can find a way to make Supreme's health bar take damage from scenes, PLEASE reach out to me asap.

- "Zev_rfl_Shoot01.pac" (Dark Shot Snipe) / (Known as "Sniper: Quick step" in Theater Mode):  
is a QTE in where Supreme uses his gun and fires 4 consecutive dark colored bullets for Sonic to dodge. A QTE most often used in a lot of Supreme showcases. Has received quite the interesting change. New QTE fail scenes were added based on Sonic's location during the 1st, 2nd, and 4th prompt. The original failure scene was not removed. It can be seen when you fail only 3rd prompt as that spot works well given where Sonic is located on the battle arena. The QTE fail for button prompts 1 and 2 are the same and the prompt buttons themselves are not changed.

- "Zev_rfl_Shoot02.pac" (Light Shot Snipe) 
Is a QTE most are familiar with Supreme using his gun and firing 4 consecutive bullets (originally colored yellow) for Sonic to parry. In this mod the bullet color was changed to blue and uses Cyber Sonic's effects when charging the gun and firing. The segments of the bullet passing by the screen happens only once as the 2nd, 3rd, and 4th gun fire will skip straight to the button prompt. The QTE fail scene has also been adjusted. Sonic will be in a different spot on the map compared to how he is originally. Since it didn't make sense for Sonic to be over water when attempting to parry, to then Sonic being in the middle of the forest when failing.

- "Zev_rfl_bitlaser02.pac" (Bit Laser) 
Another familiar scene we've all seen every time Supreme counterattacks when parrying his spin attack move while his defense drones are still active. After studying how the game handles cutscenes and tools that allow for modding, I've converted this event into a QTE. This isn't the extended 02 version I discovered some months back, but this shorter version is tweaked a bit and uses a "Press Prompt" QTE type. Though the extended versions of Bit Laser DO exist in this mod's "Retooled" QTE type option, more on that later. This game also has an unused event slot called "Zev_rfl_Bitlaser01.pac" and I cannot for the life of me figure out how to trigger the file to play in the game. It's just there, not even the executable file's coding does not mention it.

New QTEs added
With some custom HMM code, certain scenes are able to be played in the game at random.

- "test_qte_sample.pac" (One-Shot Snipe): 
Is the original game release version of Shoot02 event where Supreme uses his gun and fires at Sonic, except it only happens once that made the subsequent segments go unused, and the QTE is much slower. This event matches the same speed as the extended version built for this mod and uses the "LB + RB" button prompt to win the QTE.

- "test_sonic_walk.pac"
This is a new QTE scene that starts with an unused animation of "@attack_counter04" that has different later interactions based on passing or failing the first QTE prompt. 

- "Zev_rfl_sp00.pac"
The original scene was meant to be used for a potential special Grand Slam animation similar to how Wyvern and Knight have a special Grand Slam attack. Unfortunately, the one planned for Supreme went unused in favor for the original in-game Special Attack animation Sonic uses in most of the game and the Giganto boss. In this mod, it's been converted into another QTE slot. An alternate version of the extended "Shoot02" with pink colored bullets. The QTE type uses "The End Variant" seen in the base game's "The End" fight and has a slightly different animation. Instead of Supreme pulling out the rifle to use as a gun. He uses it as a cannon and remains hunched over and fires the weapon.

- "Zev_rfl_sp01.pac" (Wing Laser) 
As stated before, this use to be Supreme's Clap-Bite QTE, but in this mod it occupies a brand-new laser-fire QTE where Supreme uses his wings. There are 2 versions of this QTE. Options are available in the mod's settings.

* Ouranos Island Supreme Type Option: "Retooled"*

The event slot files used in the mod are the exact same, but their animations are much different here. This mod option favorites for more overhauled animations. I won't spoil too much of the newer animations here as it's better if you see them. Though I will highlight a couple of events here that were built off of the restored unused content Supreme has.

- "Zev_rfl_Shoot01.pac"
Uses the original uncut "Zev_Rfl_Bitlaser01" animation where Supreme's larger diamond turrets take their aim at Sonic and uses a laser sight lock-on. The camera is slightly edited here from the original 02 version. After Supreme locks-on, Sonic flying straight forward and looking around before Supreme fires. This has been converted into a Mash QTE type and plays during Phase 1.

- "Zev_rfl_Shoot02.pac"
Uses the original uncut "Zev_Rfl_Bitlaser02" animation where Supreme's larger diamond turrets take their aim at Sonic. Sonic flying in a different direction hoping to avoid the inferred lock-on only to realize that he can't escape Supreme's sight. Mostly unchanged from the original uncut animation, camera work included. The only difference is that Supreme has his Phase 2 pillars exposed. Also converted into a Mash QTE and plays during Phase 2. The QTE success has a different camera angle in this one compared to 01. 

- "Zev_rfl_sp00.pac"
An upgraded version of the "Restored" option of this QTE. Includes the diamond large bit turrets that blast sonic when failing the QTE.

- "Zev_rfl_Sp02.pac" (Mega Bit Laser): 
An upgraded version of the "Restored" option of this QTE. Includes the diamond large bit turrets that Supreme uses first when the struggle occurs, failing the QTE makes Supreme fire the mega laser from his mouth that sends Sonic back flying.

Cutscenes changed

- "bo4xxx.pac" 
/ "Bo4110" ... (Do Not skip if you're going to play this mod for the first time) ... has a new extended animation segment that better transitions from him holding his gun to the fight itself. Utilizes unused objects left behind in the cutscene like the Small Bit drones for Supreme and Super Sonic's animation files.
/ "Bo4160" ... (Do Not skip if you're going to play this mod for the first time) ... Has a new unique defeat animation. Rather than Supreme reeling back and slow falling to his knees, a short final scuffle was animated. Their final clash references the Showdown Trailer clash of Sonic and Giganto clashing fists. Except this time, it's Supreme. 
/ "Bo4180" ... Sonic's death scene was placed in the wrong spot entirely. Rather than being above the forest like he should be, Sonic was instead over water when the Chaos Emeralds would leave him after running out of rings. Was the intent to have Sonic drown? The death scene was also extended to have Supreme fire one last shot at Sonic and send him flying away before the game cuts to black.

--------------------------------------------------------------------------------------------------------------------------------------------------
Titan: The Supreme End (aka "Riflebeast")
Some work was done to this boss as well. Though not to the extent that I did for the original Supreme. However, I can highlight what I've done for him.

- attackPattern:
* Adjusted the attack pattern so that Supreme will claw-swipe every 2 orb attacks. 
* Also adjusted the camera panning so that the trees aren't in the way. However, if you're too close to Supreme you may not be able to see the orbs themselves, so it's best to hang back to see the orbs when they fire. If this change becomes too much of a hassle in the fight, I'll see if I can work out a fix.

- attackPatternAfter:
* This boss has 4 unused "AT_Himing" attack slots that are utilized for this fight's Phase 2. 

- "bo6xxx.pac" (Realtime)
* "bo6110" ... unchanged. (However,...)
* "bo6120" ... has a slight change towards the end of the cutscene and a change to when SS2's model will spawn.
* "bo6125" ... didn't mess with it. (...another mod will...)
* "bo6130" ... didn't touch these. (...add specific dialogue...)
* "bo6140" ... Fixed a rendering error in which regular Super Sonic is shown after Eggman grabs Supreme's gun. So now SS2 and whatever mod skin uses SS2 should appear.
* "bo6160" ... remains the same. (...to certain cutscenes...)
* "bo6165" ... slightly changed cutscene position to make it look like Sonic is slamming into the barrier with the large laser orb when viewing in Realtime. The camera angle Sonic returns into his SS2 form.
* "bo6170" ... also unchanged.  (...with unused captions.)
* "bo6180" ... A new death animation was implemented should you lose your rings. The same location problem bo4180 had was addressed here too.
* "bo6190" ... received a significant fix in which Eggman's scope display is shown for the whole cutscene, the only catch is that the shot in which Eggman is looking up at Supreme with the reticle effects is the only pre-rendered segment of the entire cutscene as I couldn't figure out how to show in its proper spot in Realtime.

- "Zev_parrymiss_riflebeast.pac" 
This QTE was adjusted to remove a segment that didn't make a lot of sense. Since You're locked at the center of the arena when parrying Supreme's claw swipes, it didn't make sense for this QTE to start from the edge of the forest back to the center. Though the animation was moved somewhere else, so it's not completely cut.

- "Zev_blow_rifleboss.pac" 
This QTE has been significantly updated. Not the initial parts, but the "Blowmiss_Riflebeast" animations should you fail at the start. Super Sonic 2 will have his aura back when Supreme lands on the ground to grab Sonic and during the mash struggle. When you win the mash prompt a new animation will play in which Supreme will try to attack Sonic just to be kicked back down, a better transition to Supreme falling back down to restart the QTE. When you fail the mash struggle, Supreme will instead throw Sonic instead of throwing him to the floor.

These changes were made so that it's not the exact same as "Parrymiss" Though if you want those original animations, the option is there albeit fixed so that Sonic doesn't mysteriously disappear after freeing himself from Supreme's grip.

- "Zev_sp_riflebeast.pac" 
Also, in Realtime. No pre-rendered shots here. If you use Hyper Sonic mod skins, I implore you to check out this mod's "Hyper Sonic skin" option when looking through the Final Horizons setting.
