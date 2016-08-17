# Character controller

The Character controller allows for some specific functionality, useful to have when moving around a character in your world, that needs to interact with colliders, but also needs to respond to user input (such as keyboard, or mouse inputs) in an interactive way.

## Character controller properties

Property              | Description
----------------------|---------------------------------------------------------
Collision group       | Defines to which collision group this entity belongs.
Can collide with      | Defines with which groups this entity can collide.
Collision events      | Toggles whether this entity received collision events.
Can Sleep             | Toggles whether this entity can sleep. ??
Restitution           | Defines how much this entity absorbes energy, and therefore bouncyness. ?? How does this work ?? values ??
Friction              | Defines how much surface friction this entity has.
Rolling Friction      | Defines how much rolling friction this entity has.
Ccd Motion Threshold  | Continuous collision detected velocity threshold - this value indicates at which velocity the Ccd kicks in to prevent errors for objects that are moving very fast.
Ccd Swept Sphere Radius | Continuous collision detected sphere radius - this is the radius of the bounding sphere between 2 physics steps.
Step Height           | The maximum height the character can step onto.
Fall Speed            | ?? The speed at which the character will fall. This is the amount gravitational pull.
Max Slope             | The maximum slope the character can climb. ?? In degrees. 
Jump Speed            | The size of the jump force.
Gravity               | ??