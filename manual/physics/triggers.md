# Triggers

<div class="doc-incomplete"/>

Triggers allow you to trigger an event when a certain object enters a trigger area / volume. In order to create a trigger you need to take the following steps:

**To create a trigger:**

1. Add an Entity to your scene. This can be a model, or a non graphical Entity like a collider

2. Select the Entity and click 'Add component' in the Property grid.

3. Add a static collider object

4. In the static collider section, check the 'Is Trigger' option. This allows for physics objects not to actually be affected by the collision with this collider, and just pass through it.

Now a trigger has been created. To handle the trigger, we need to add a script.

**Handle trigger event with script:**

  1. Create a an Async script in your game project

  2. Open the script in Visual Studio and enter the following sample code:

```
    using SiliconStudio.Xenko.Engine;
    using SiliconStudio.Xenko.Physics;
    using System.Threading.Tasks;
    using SiliconStudio.Core;
    using SiliconStudio.Xenko.Engine.Events;

    namespace VolumeTrigger
    {
        public class Trigger : AsyncScript
        {
            public override async Task Execute()
            {
                var trigger = Entity.Get<PhysicsComponent>();
                trigger.ProcessCollisions = true;

                // Start state machine
                while (Game.IsRunning)
                {
                    // Wait for entities coming in
                    var firstCollision = await trigger.NewCollision();

                    // Now do something, your trigger has been hit!

                    // Now wait for entities exiting
                    Collision collision;

                    do
                    {
                        collision = await trigger.CollisionEnded();
                    }
                    while (collision != firstCollision);
                
                    // Now do something else, the trigger has been deactivated
                }
            }
        }
    }
```

  3. Finally put in the your code in the above example, to handle what happens when the trigger has been activated and de-activated.
