# MAVERICK
Finalized Build/Source Code of MAVERICK, a game created by "Atlas Development" for the 2024 Borderlands Glitch Game Jam. Won *Most Technical* Award & 4th Place Overall. [✈️]

<p align="center">
<img src="https://github.com/Azaze7/MAVERICK/blob/main/ReadMeAssets/Maverick_TitleScreen.png" height="375px"> 
</p>

## 🔎 Table of Contents.

1. What is MAVERICK? What were our Design Decisions?
2. Team Composition [Atlas Development]
3. What Files are Enclosed Here?
4. Video Demonstration.
5. SteamOS Integration.
6. The Cutting Room Floor.
7. Closing Thoughts.

##  What is MAVERICK? What were our Design Decisions?
* Powershell-Empire was an open-source post-exploitation agent that ran through Windows Powershell.
* It allowed for a user to generate attack scripts for use against other Windows machines, MacOS, or Linux subsystems.
* It is not offically maintained as of August of 2019, but a fork was used as a base for the creation of this cybersecurity excercise.

### (Unofficial) License Choice
* Since the prompt of this GameJam was to choose a movie or TV show from the late 80's through early 90's to base our game off of, we started by making a list as a team of what media we enjoyed from the era.
* We took team votes to decide which games were feasible given the time constraints/looked fun to create, then recursively struck bad ones off of our list.
* Some titles discussed, their potential genre, and the reason they were struck are:


| *Title* | *Genre* | *Struck Reason* |
|----------|----------|
| The Evil Dead (1981) | Survival Horror | Too many unique Assets to make something nice. |
| Indiana Jones & The Raiders of the Lost Ark (1981) | 2D Platformer | Too many unique Assets to make something nice. |
| Karate Kid (1984) | Fighting Game | Too many unique animations, not our forte since were all in CS. |
| Back to the Future (1985) | 2D Platformer/Driving Game | Lack of Interest. |
| [⭐] Top Gun (1986) | 2D Shooter/Bullet Hell | Won The Vote! |
| Space Balls (1987) | Ship Simulator | Too much code to make a fun simulation. |
| Forest Gump (1994) | Endless Runner | Lack of Interest. |


### Naming Conventions
* Due to the rules stating that we were *NOT* allowed to directly adapt the movie, we chose to make our game a prequel to the original Top Gun Film, when the main character Pete “Maverick” Mitchell was still in Flight School, using a simulator.
* The name of the game, MAVERICK, was chosen to satirize the weird naming conventions that are tied to movie franchises like Rocky and Rambo. (Such as Rocky 6 being called “Rocky Balboa” and Rambo 4 being called just “Rambo”).
* This made our game fit neatly into Top Gun's Timeline, with it now being:
* MAVERICK -> Top Gun -> Top Gun: Maverick.

### "Cabinet" Design
* Since MAVERICK takes design inspiration from retro arcade games, we decided to copy the way that those games are played nowadays.
* Emulated collections of arcade games are usually played on modern TVs or monitors, which are much wider than the arcades of old.
* We decided to add side art to border MAVERICK, pretending it was a real arcade game when it's in play.
* You may have seen this before in retro collections such as NAMCO Museum.

<p align="center">
<img src="https://github.com/Azaze7/MAVERICK/blob/main/ReadMeAssets/PAC-MAN_Arcade_Banner_Example.png" height="200px">
<img src="https://github.com/Azaze7/MAVERICK/blob/main/ReadMeAssets/MAVERICK_Arcade_Banner.png" height="200px">
</p> 

### A 2-level Approach.
* In order to teach players who may have never played a 2D shooter, the first level was set to be a tutorial with basic graphics. The colors are purposely kept simple with vectors to tie into our plot of Maverick still being in Flight School.
* After the first level is completed, the difficulty was to be increased and a more impressive presentation would also follow.
* We were only trying to do a 2 level vertical slice due to the strict time constraints.

### Healthbar & Difficulty.
* In order to ensure MAVERICK was able to be completed by everyone who played it on the show floor, we took a more "modern-day approach" to the game's difficulty.
* While MAVERICK did take a ton of inspiration from retro arcade style shooters, we did not want it to feel like it was designed to take your quarters away, nor overly frustrating to even a novice gamer.
* To accomplish this, we removed the concept of lives so that everyone could just play the game, and respawn after a short while when they died. We did NOT want anyone to reach a GAME OVER state early. (This concept is implemented in many modern games, such as Celeste or Super Mario Odyssey).
* We also increased the number of hit points the player ship could take for the sake of the demo. It was increased from 5 to 25, which in practice made it almost impossible for anyone to even see their ship blow up, especially since this was originally a tutorial stage.
* We had very few people die while playing MAVERICK on the show floor, and when they did they respawned very quickly to keep the game fun.
* *If MAVERICK was to be retooled, rebranded, and then released as a proper videogame, the hitpoints would be decreased to a more "challenging" level.*


## 🎏 Team Composition [Atlas Development]

**This Project was completed with the assistance of *four* group members!**

* Awarded [*4th Place Overall*] & [*Most Technical Award*].

Special Thanks to All Team Members!

[William Dunlap](https://github.com/unit098 "William's Github") - *Code Lead*: Major Game Logic, Level Loading, Enemy Behaviors, Smoke Trail System, & Bullet System.

[Gilbert I. Guzman](https://github.com/Azaze7 "Gilbert's Github") - *Team Coordinator*: Main Menu System, Game Logos/Emblems, Powerup Design, Code Assistance, SteamOS Support/Artwork, & Communicated with Staff.

[Dante Lopez](https://github.com/dragons6612 "Dante's Github") - *Art Support*: Assisted In Creation of all Assets, Consulted on Jet Design/Pixel Art for "realistic" level, & Side Playtester.

[Jesus Torres](https://github.com/jatorresdom "Jesus's Github") - *Lead Composer*: Composed All Music, Created Ending Screen, Ending Artwork, & Main Playtester.

[Zachary Whittman](https://github.com/Zachary-Wittmann "Zachary's Github") - *Art Lead*: Requested Assets from Members, Taught GIMP to Team, Code Assistance, Background Creation and Effects, & Powerup Design. 

<p align="center">
<img src="https://github.com/Azaze7/MAVERICK/blob/main/ReadMeAssets/Atlas_Development_Team_Photo.jpg" height="375px"> 
</p>

## 🗂️ What Files are Enclosed Here?

| Filename | Type | Description | 
| --------------- | --------------- | --------------- |
| DemoPresentation_Software... | .pptx | PowerPoint used during live demo. |
| InfoPresentation_Software... | .pptx | PowerPoint used to inform audience about PowerShell-Empire. |
| Poster_Software... | .pptx | PowerPoint that contains a single slide "poster" about PowerShell-Empire. |
| Exercise_Software... | .docx | Word Document that contains instructions on how to use PowerShell-Empire, in the same format used in CS4177. |
| Final_Powershell_Command_Encoded_Base64 | .ps1 | Script used in Windows PowerShell. It contains instructions to take control of a Windows 7 Professional Virtual Machine. |
| Powershell_Empire_Screenshot | .png | Sample Screenshot of Kali Linux & Windows 7 Professional. Used for this README. |

## 🎞️ Video Demonstration.

* A video demonstrating a full run of the one level we completed for our vertical slice was recorded by myself for this project.
* Since it is too big to upload here, it can be found at this link:
  * https://www.youtube.com/watch?v=DJutJYl7XlY 

## 🕹️ SteamOS Integration.

* Since Maverick was made playable on both standard computers and the Steam Deck, artwork was created so that it wouldn't look out of place next to other video games.

<p align="center">
<img src="https://github.com/Azaze7/MAVERICK/blob/main/SteamGridAssets/Maverick_SteamOS_Demonstration.gif" height="375px"> 
</p>

* It is a great source of pride that our team's game is able to sit next to games that were part of both our childhood and adulthood.
* If you would like to use these artworks for your copy of MAVERICK, please look at the [SteamGridAssets](https://github.com/Azaze7/MAVERICK/tree/main/SteamGridAssets "Steam Grid Artwork") folder. :)

## ✂️ The Cutting Room Floor.

* Due to the strict timing of the Game Jam, we were unable to fully complete our original vision of MAVERICK.
* MAVERICK ended up having to be a single level, with the second level being completely struck.

### Second Level & "Realistic" Artstyle.
* The original intention was for the green line level (level 1) to act as a tutorial, teaching the player how the game worked since it was a "simulation".
* This tutorial took inspiration from military radar equiptment and games like Atari® BattleZone, which used simple lines and vectors for their visuals.
* After the first level was completed, a secondary level was to be loaded in with a more "realistic" artstyle and harder enemies. This level was to have fully animated water and sandy beaches, along with an additional, already completed but unused song.

* Below are some of the additional sprites we had created for it. Keep in mind, in our code every single sprite had the same hitbox regardless if it was in the tutorial or real version of the level.
* (Every asset we created had a tutorial and realistic version created, though they went unused.)

| | Tutorial | Realistic |
|----------|----------|----------|
| Player Character [F-14 Tomcat] | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/Tutorial_Ship_Player.png" > | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/F-14_Tomcat_Player.png" > |
| Enemy (Side-to-side) [MIG-28] | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/MIG-28_Tutorial_Ship_Enemy.png" > | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/MIG-28_Enemy.png" > |
| Enemy (Stationary Missle) [MIG-29] | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/MIG-29_Tutorial_Ship_Enemy.png" > | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/MIG-29_Enemy.png" > |
| Enemy (Divebombers) [YAK-141] | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/YAK-141_Tutorial_Ship_Enemy.png" > | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/YAK-141_Enemy.png" > |
| Enemy Missle     | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/Enemy_Missile_Tutorial.png" > | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/Enemy_Missile_Real.png" > |

### Powerups.
* It was the team's intention that enemies that were destroyed would periodically drop powerups.
* These powerups were loosely based off the Top Gun© Movie, and included things like a pair of avaitor sunglasses and a volleyball.
* Their sprites and intended functions are shown below.

| | Tutorial | Realistic | Function |
|----------|----------|----------|----------|
| Volleyball | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/Volleyball_Tutorial.png" > | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/Volleyball_real.png" > | Summoned an additonal jet that would fly next to yours for double firepower. (Inspired by double ships in NAMCO's Galaga.) |
| Sunglasses | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/sunglasses_Tutorial.png" > | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/sunglasses_real.png" > | Created a shield that would be at the front of the player's jet. This shield could be used to block enemy fire for a short while. |
| Maverick Emblem | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/MaverickEmblem_Tutorial.png" > | <img src="https://github.com/Azaze7/MAVERICK/blob/main/SpriteComparisonAssets/MaverickEmblem_Real.png" > | Made all shots fired by the player into missles for a short while. (Design based powerups in Konami's Contra.) |

## 🚪 Closing Thoughts.

