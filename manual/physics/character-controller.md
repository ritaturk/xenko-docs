# Character controller

The Character controller allows for some specific functionality, useful to have when moving around a character in your world, that needs to interact with colliders, but also needs to respond to user input (such as keyboard, or mouse inputs) in an interactive way. The character controller handles similar to a rigid body collider with the 'Is Kinematic' option switched on.

## Character controller properties

Property              | Description
----------------------|---------------------------------------------------------
Collision group       | Defines to which collision group this entity belongs.
Can collide with      | Defines with which groups this entity can collide.
Collision events      | Toggles whether this entity received collision events.
Can Sleep             | Toggles whether this entity can sleep.
Restitution           | This coefficient defines how much energy remains after a collision for the objects to rebound from one another. Typical values range from 0...1 where 0 means all energy is lost, and 1 means all energy is preserved and the objects will move away from each other at the same speed they collided.
Friction              | Defines how much surface friction this entity has.
Rolling Friction      | Defines how much rolling friction this entity has.
Ccd Motion Threshold  | Continuous collision detected velocity threshold - this value indicates at which velocity the Ccd kicks in to prevent errors for objects that are moving very fast.
Ccd Swept Sphere Radius | Continuous collision detected sphere radius - this is the radius of the bounding sphere between 2 physics steps.
Step Height           | The maximum height the character can step onto.
Fall Speed            | The maximum fallspeed. If the speed at which a character falls towards the ground exceeds this it is capped to this value.
Max Slope             | The maximum slope the character can climb. ?? In degrees. 
Jump Speed            | The size of the jump force.
Gravity               | The amount of gravitational pull.
