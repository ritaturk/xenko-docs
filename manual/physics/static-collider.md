<div class="doc-incomplete"/>

# Static collider

A static collider is an object that itself is not affected by forces like gravity or collision and therefore doesn't move (i.e. static), but does affect rigid body objects when they collide with it. This type of collider is typically used for static game objects such as a wall or a floor object.

**To create a static collider:**

1. Starty Game Studio with the empty Game project

2. Select the ground (gray plane) in the Scene Editor

3. Click 'Add component' in the Property grid

4. Select 'Static collider'

5. Now find the created static collider in the 'Property grid', and expand to view the collider properties

6. Select the '+' icon behind 'Collider Shapes' and select 'Infinite Plane'

Now you've created a static collider for the ground plane in the empty Game Studio project, which allows other physics objects to interact with it.

## Static collider properties

Property              | Description
----------------------|---------------------------------------------------------
Collision group       | Defines to which collision group this entity belongs.
Can collide with      | Defines with which groups this entity can collide.
Collision events      | Toggles whether this entity received collision events.
Can Sleep             | Toggles whether this entity can sleep.
Restitution           | Defines how much this entity absorbes energy, and therefore bouncyness.
Friction              | Defines how much surface friction this entity has.
Rolling Friction      | Defines how much rolling friction this entity has.
Ccd Motion Threshold  | Continuous collision detected velocity threshold - this value indicates at which velocity the Ccd kicks in to prevent errors for objects that are moving very fast.
Ccd Swept Sphere Radius | Continuous collision detected sphere radius - this is the radius of the bounding sphere containing the position between 2 physics frames.
Is Trigger            | Toggles whether this entity is a trigger.