# Game Build Differences

When a game is released and when a game is built are two different things.

The game release dates per region came from [www.wikipedia.org/wiki/Shadow_the_Hedgehog_(video_game)](www.wikipedia.org/wiki/Shadow_the_Hedgehog_(video_game))

These build dates came from [https://tcrf.net/Shadow_the_Hedgehog#Build_Dates](https://tcrf.net/Shadow_the_Hedgehog#Build_Dates)


### Region Release Dates

|Region|Release Date|
|--|--|
|NA|November 14, 2005|
|PAL / EU|November 18, 2005|
|JP|December 15, 2005|

### Game Build Dates

|Version|Build Date|
|--|--|
|GameCube (US)|Oct 10 2005 23:48:24|
|PlayStation 2 (US)|Oct 12 2005 14:56:41|
|PlayStation 2 (EU)|Oct 16 2005 12:09:34|
|PlayStation 2 (JP)|Oct 16 2005 12:09:34|
|GameCube (JP)|	Oct 16 2005 15:45:51|
|Xbox (US / EU / JP)|Oct 16 2005 15:49:12|
|GameCube (EU)|Oct 20 2005 11:17:41|

So what we see here is that there's about a month between the final build of the games and their release.  But we also see that they were not built at the same time.  

While not always the case with games, there are a handful of differences between games these builds depending on when they were built, even if they were released at the same time.

For example, the versions build on Oct 16th and later have the powerful Chaos Control Glitch patched. Making the US GameCube and PS2 versions the only ones that can perform that glitch.

The Oct 16th and later versions also have a few minor level object (layout) differences, extra objects are added as documented below.

### Oct 16th Layout Changes

|Stage & Type|Change|Layout File|
|--|--|--|
Glyphic Canyon (All)|Extra Killplane Collision (6) on Secret KeyDoor route|stg0201/stg0201_cmn.dat|
Cryptic Castle (Expert)|ChaosControlStop Trigger at Chao Room / Dark route|stg0300/stg0300_hrd.dat|
The Doom (All)|Bugfix/GUN Robot (170) sets RenderDist 7 -> 5 to prevent it falling through floor, *possibly also "Unknown" as well|stg0401/stg0401_cmn.dat|
Mad Matrix (Normal)|Unknown|stg0403/stg0403_nrm.dat|
Air Fleet (All)|Unknown|stg0501/stg0501_cmn.dat|
Air Fleet (Expert)|ChaosControlStop Trigger x2 for blocked door / routes on Expert|stg0501/stg0501_hrd.dat|
Iron Jungle (Expert)|ChaosControlStop Trigger at RailSplit / Dark upper route|stg0502/stg0502_hrd.dat|
Lost Impact (All)|9 Extra Objects, 7 are SolidCollision Triggers, 1 Extra GUN Beetle and GUN Soldier at Checkpoint 8|stg0504/stg0504_cmn.dat|
GUN Fortress (All)|Unknown|stg0600/stg0600_cmn.dat|
GUN Fortress (Expert)|Two ChaosControlStop Triggers on upward Hero route areas|stg0600/stg0600_hrd.dat|
Lava Shelter (Expert)|ChaosControlStop Trigger on Hero route|stg0602/stg0602_hrd.dat|
Final Haunt (Destructibles)|Unknown. Note: Both have a Black Oak (Giant) which is abnormal for .ds1 files|stg0604/stg0604_ds1.dat|
Final Haunt (Expert)|4x Duplicate Black Oak (x2 on Oak # 1, x2 on Oak # 3), x3 Platform Duplicate, x3 ChaosControlStop Triggers at Dark Route Flying Sections|stg0604/stg0604_hrd.dat|

The most significant changes are Final Haunt (Expert), The Doom (All), and Lost Impact (All).

**Final Haunt** contains duplicates of objects found in the cmn layout, in the hrd (expert mode) layout. There are 4 extra Black Oaks stacked into their original object and 3 extra platforms stacked into original objects. Likely these duplicate objects were a copy/paste mistake while the ChaosControlStop Triggers were added.

**The Doom** lowers the render distance of the GUN Robot with LinkID 170, located right after the 6th checkpoint in the proceeding elevator room. This is a significant change as pre-Oct 16 builds of the game have to warp away with the checkpoint and back again to get this robot to spawn for the mission The Doom Dark.

**Lost Impact** adds extra SolidCollisions to the ceiling of some rooms, preventing out of bounds ceiling jumps via spindash jump- none of which are currently used in runs anyway. Additionally, there is an extra GUN Beetle and GUN Soldier at the 8th checkpoint.

**Other stage changes** consistent primarily of adding in ChaosControlStop Triggers that act as quick bugfixes. These prevent players from going the wrong way in Expert Mode while using Chaos Control. Ex: Cryptic Castle Dark route instead of Normal route while in Expert Mode.

**Unknown** changes mean the object counts are identical across versions, but there is a checksum difference. Likely an object was tweaked: position, rotation, object parameters (which weapon an enemy holds, how they behave, etc). Alternatively, it is possible an object was swapped out entirely for another object (ex Metal box for Wood box). These specifics are not determined, it is only known the count is the same but there is a mismatch regardless.