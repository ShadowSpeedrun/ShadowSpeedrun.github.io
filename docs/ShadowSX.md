![](/img/S-SX-Logo.png)

## Download on GitHub

#### [Click here to visit the GitHub Release page](https://github.com/ShadowSpeedrun/ShadowSX/releases)
<br/>
<u>You will need to provide your own clean rip of the Shadow ENG NTSC ROM to run with the emulator.</u>

<u>The only files provided on GitHub are the configuration files needed to apply the settings and changes to run Shadow SX.</u>

<br/>

## What is Shadow SX
Shadow SX is a combination of a ROM hack of the ENG NTSC version of Shadow the Hedgehog and the use a specific setup of the Dolphin Emulator that aims to provide quality of life changes for improving the speedrunning experience without any changing of the core gameplay.

Although this website started as a means of consolidating and proving data for the console releases. Everything you see on this site should apply to both the console versions and Shadow SX.

Due to changes to the game code and the use of perforance enhancing features in the Dolphin Emulator, Shadow SX will be considered it's own thing seperate from the original console releases.  Seperate Leaderboards for any of the categories or levels will be provided at a future time.

This current release is considered an ALPHA and is ment to get a feel for how everyone is able to setup and play this version.  I will be expecting changes to the emulator and ROM hack code as we move into BETA and then into a definitive version.

If you record and upload any footage of Shadow SX, please be sure to properly label the video as the SX version including if it's ALPHA or BETA or whatever to help prevent confusion for future viewers / runners of the game.

<br/>

## Changes Compared to the Original

The following changes have been made to the game code:

### Checkpoints no longer pause the In Game Timer (IGT)

The game will no longer pause the timer while in the checkpoint menu.  This prevents the use of the checkpoint for saving IGT while waiting for another in game event to playout.  More important though, is that this change allows the use of IGT timing for runs that utilize the Chaos Control Glitch.

### Deaths no longer reset the IGT to the last checkpoint time

One of the biggest headaches when timing IGT runs on console was having to manually calculate the time from deaths to checkpoints.  With this change, the time continues without interuptions after death.  The time you end the level with is the final time now.

### Restarting a stage during a "Story Mode" playthrough no longer resets the IGT.

This change, while applies to every level, is mainly targeted to the shorter Boss Fights where one might reset quickly early on if a setup doesnt go to plan. Like with the Death fix above, the timer will simply continue form that point on until the end of the level or boss fight.  

This does NOT apply to levels or bosses that are started with "Select Mode" as this would quickly become annoying for Individual Level (IL) runs and attempts. This applies only for Normal Story, Last Story, and Expert Mode playthroughs.

### Overclocking with Dolphin Settings

Since Shadow SX and the console Shadow releases will not be comparable, Shadow SX will utilize the Dolphin Emulator's ability to run at a higher clock frequency for better perforance and a smoother experience.  This should play similar to running on Nintendont on a Nintendo Wii.

### Improved Loading Times

The Dolphin Emulator has a setting to allow faster reading of the ROM data.  So instead of having to match a similar rate to the GameCube disc drive, the emulator can read and load data much faster allowing vastly shorter load times.  Normally getting from the end of Westopolis to the beginning of Glyphic Canyon takes a little over a minute on Wii.  With this change, it now takes 48 seconds.

<br/>

## Planned Roadmap for future changes

### ALPHA
The plan with ALPHA is to get feedback on the current changes and how the Dolphin Emulator setting work to find something the is fair and works for everyone.  There may be a mini update during this time to fix issues or provide smaller changes.

### BETA
The main plan for BETA is to improve the setup and managment process. Setting up ALPHA is currently very manual and requires knowledge of properly managing files and a roundabout way of booting the game.  By time BETA is finished, there should be a much cleaner and automatic setup of the required files. 

While ALPHA will allow any recent Dolphin Emulator to run the game, BETA will lock this down to a specific version of Dolphin that will be modified to fit the needs of Shadow SX and keep everyone as equal as possible. With this, a nicer way to manage save data and shortcuts to Dolphin configuration settings like Controller Settings will be done at this time.

BETA will also be the start of game texture swapping to make it much more clear to the viewers of the game that this is Shadow SX and not the console Shadow release.

### Full Release
Once everything is ironed out and finished in BETA, a proper release will be made.  At this point a leaderboard should be available to track runs of the game.