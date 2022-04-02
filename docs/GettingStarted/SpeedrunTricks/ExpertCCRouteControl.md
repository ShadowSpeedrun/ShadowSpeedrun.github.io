#Expert Chaos Control Route Control

If you are not aware, different Chaos Control paths/branches/splines can sometimes be taken depending on which partner you have out.

For example, Glyphic Canyon takes the full circular route at checkpoint #5 if Black Doom is out. 
It skips it if Knuckles or No Partner is out.
Seen here:
![type:video](https://www.youtube.com/embed/UQkjTtP7yvI)

This brings us to Space Gadget, which allows us to take the Dark Route or Hero Route depending on which partner we have out. Initially it was thought Expert mode disables the mission byte flags. Specific positioning was used to get the correct CC branch in Expert mode to get to the faster route in Space Gadget.

However I found only the D-Pad mission flags were disabled. You can set the mission flags in the pause menu.
This is because the pause menu code is the same as normal mode, only the images are different.

Thus we can set ourselves to instantly take the Hero spline in Space Gadget Expert:

1. Pause the game
2. Press "down", highlighting "restart" 
3. Press "right", setting the 'hero' flag
You'll know it worked because the "restart" will move back up to "resume" with no noise

4. Press "A" (or equivalent for non-GameCube, not the Start or pause/unpause button!)

This video shows the default behavior and after setting the 'hero' mission flag:
![type:video](https://www.youtube.com/embed/CzB57zg_BiQ)

This trick also results in some expert stages having regular partner dialog if you perform this early. Notably Digital Circuit has lots of left over voice lines from Normal Mode lingering in Expert Mode if you enable the mission flag.