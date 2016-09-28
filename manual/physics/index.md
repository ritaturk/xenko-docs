# Physics

<div class="doc-incomplete"/>

The Xenko engine provides you with tools to realistically simulate physics in your game or application. The Xenko Physics engine simulates forces such as gravity and collision in a natural convincing way. With the built-in components it's easy to enable physics for your entities and allow them to interact with eachother.

This section will show you how to enable physics in Game Studio, how to use the correct physics component for your needs, and how to apply forces to an Entity through scripting. We will also show you how to use triggers, which allow you to trigger an event when an object enters a certain space for instance.

## Basics

Physics simulation is the process of simulating how physical objects interact with each other, and how they react to forces such as gravity or collisions. In Xenko we refer to physics objects as **Colliders**. In Xenko we use 2 types of colliders:

* [Rigid body colliders](rigid-body.md)
* [Static colliders](static-collider.md)

Rigid body colliders will move based on the forces (such as gravity and collisions) applied to them. Static colliders will cause a collision when a rigid body collider collides with it, but will not move themselves. Typically static game elements such as walls and floors will be static colliders, and game elements (such as players, cars, etc.) will be rigid body colliders.

Entities with colliders attached to them, should not be moved directly by their **Transform** property, but instead should be manipulated by applying forces.

However if your entity is controlled by script or animation most of the time, but only sometimes needs to interact with other physics objects, you can set the **Is Kinematic** flag for a Rigid body collider. The collider will still raise collision events, but will not respond to them. When the collider needs to start interacting with other colliders again, simply disable the **Is Kinematic** flag in your script. When **Is Kinematic** flag is set, you will be able to move the Entity and thus the rigid-body from the **Transform** itself.
An example when to use this, is for instance, when a player character is mostly controlled by animation and user input, but needs to respond in a convincing way when the player is hit by a particular object. 

Besides collision detection and logic, the physics simulation in Xenko offers:

* [Triggers](triggers.md) - these are objects that detect collision, but no not affect the objects that collide with it. This allows for script logic to be linked when an object enters (collides with) another object.
* [Raycasting](raycasting.md) - this is the process of tracing a line (ray) through the scene, to find out which objects intersect with this ray. This can be useful for instance to find objects in the scene based on the screen position where the user clicks is mouse, or finding out which objects are affected by a fired projectile.
* [Character controller](character-controller.md) - this controller can be typically used to move around characters or players in a 2D or 3D world. The Character controller allows for some specific functionality, useful to have when moving around a character in your world, that needs to interact with colliders, but also needs to respond to user input (such as keyboard, or mouse inputs) in an interactive way.
* [Constraints](constraints.md) - constraints can be used to link colliders together with certain conditions. An exampleof this is: limbs that have a limited amount of rotation to be realistic.  
