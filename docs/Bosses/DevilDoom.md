# Devil Doom

## General Info 
* Starts with 200 HP
* TODO: Add the health per wing (which has no affect on boss HP)
* A non-charged chaos spear does 6 damage
* A fully charged chaos spear does 20 damage (approx 3 seconds to fully charge)
* The cue for eye vulnerability is when the current head tracks/looks at Shadow while near. However, during some other states the head may not track while the boss is vulnerable.

However, no other chaos spear states exist in between. It turns out every ms spent charging adds to this amount - yes, even holding for 0.01 seconds produces a result of 6.311096 damage. It is not necessary to have the effect change color.

The chaos spear charging blue/yellow particle effect (before the blue circle) will do 15 damage and takes ~1.5s to reach this state - which is half the time of a full spear for only 5dmg less.

Unfortunately, to achieve an optimal time of <=0:50 (collecting no rings) requires 10 fully charged 20s hits, and due to the boss invulnerability period the window to achieve this time is extremely precise.

### Player Spawn Location
Due to an oversight in the Super Shadow Fly state, the player's position is not reset when you perform a restart. You can utilize this to change your starting position.

### Phase 2 Differences (Half Health)
The angle which triggers Wing Guard is wider, requiring the player to have a smaller angle of attack to the eye.

## Boss States

### Body Change
Occurs when the Player does any damage to the eye.
The eye switches which head it lands in. Takes (TODO: VERIFY time per change) 5 seconds per change.
Completely invulnerable during this state.

### Chaos Control
Occurs if Shadow is too close, too far away, or the boss was attacked without an active target/lock on to Shadow.
Devil Doom has two positions it can be in at any given time. These two points are alternated between each Chaos Control.
The exception is at stage init / stage restart, the boss will be in the center, between these two points. The boss will never return to this point once it warps without restarting the stage.
Devil Doom will warp to the opposite point when activated.

### Wing Guard
Occurs if an attack is performed from an angle too far left/right of the eye. If Devil Doom's left/right wing are not destroyed, the wing will block the attack. This state can be exploited to extend other state durations. 

### Black Stone
Devil Doom will perform the standard fly/idle animation. Stones will spawn out of the ball attached to Devil Doom.
Fully vulnerable while in this state, and easy to hit.
These stones have various formations that can be created (scattered, circle, line).
The stones will shoot lasers at Shadow's current position.

### Fire
Devil Doom will quickly charge a flame breath attack and spew fire in a straight line at Shadow's current position.
Invulnerable while the animation is active.

### Psycho Attack
Devil Doom will raise debris (which when destroyed, give Dark points) and Item Balloons (which when destroyed, give 20 Rings).
During which his arms are raised upward.
His eye is vulnerable during this, however due to the animation and targetting system it will not be possible to hit his eye until his hands reach the peak height.
Guaranteed to follow up with Psycho Throw attack.

### Psycho Throw
Can only occur if debris from Psycho Attack are still present. Devil Doom will perform a throw animation. This animation can be either left or right arm instances, depending on where Shadow is located. One of the pieces of debris will be flung directly targeting Shadow's current position. Upon the player getting close to the boss, all the remaining objects will perform a cross section to reach the opposite point of their current positions. Eventually after a certain amount of time (TODO: add time) the remaining debris will fall.
TODO: check eye vulnerability period/hit feasibility