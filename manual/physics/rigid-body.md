# Rigid body

Rigid body simulation refers to the simulation of physics for objects that do not deform. Rigid body simultation can be used for collision between objects, and for objects that need to repsond to incoming collisions.

**To enable rigid body simulation for an entity:**

1. Start Game Studio with the empty Game project

2. Select the Sphere in the Scene Editor

3. Click 'Add component' in the Property grid

4. Select 'Rigidbody'

5. Now find the created Rigidbody in the 'Property grid', and expand to view the Rigidbody properties

6. Select the '+' icon behind 'Collider Shapes' and select 'Sphere'

Now you've created a Rigidbody for a sphere, the sphere and ground plane are ready to interact with each other. Run your game and you can see how the sphere is affected by gravity and collides with the plane.

## Rigid body properties

Property              | Description
----------------------|---------------------------------------------------------
Collision group       | Defines to which collision group this entity belongs.
Can collide with      | Defines with which groups this entity can collide.
Collision events      | Toggles whether this entity received collision events.
Can Sleep             | Toggles whether this entity can sleep. *
Restitution           | Defines how much this entity absorbes energy, and therefore bouncyness.
Friction              | Defines how much surface friction this entity has.
Rolling Friction      | Defines how much rolling friction this entity has.
Ccd Motion Threshold  | ??
Ccd Swept Sphere Radius | ??
Is Trigger            | Toggles whether this entity is a trigger.
Is Kinematic          | Toggles whether this entity is kinmetic, i.e. interacting with other physics objects.
Mass                  | Defines the mass of this entity in KG.
Linear Damping        | Damping factor for directional forces.
Angular Damping       | Damping factor for rotational forces.
Override gravity      | Use custom set gravity vector.
Gravity               | Defines a custom gravity vector.
Node Name             | ??
