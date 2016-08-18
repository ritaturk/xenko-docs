# Introduction to using Prefabs

Prefabs are essentially collections of various kinds of Entities that can be re-used in your project, and need a single point where they can be configured and maintained. Prefabs are ideal to use for things like scenery (trees).
Because all instances of a prefab are based on the original prefab, changing any properties or contents of the prefab will cause all instances of this prefab to be altered.

## Added a prefab to the scene in Game Studio

Once you've created a Prefab, you can easily drag and drop the Prefab from the Asset view into the Scene editor, like any other Asset.

## Using Prefabs from script

In order to use prefabs at runtime, you need to intantiate them. Let's assume we have a Prefab called 'MyBulletPrefab' located in the root of our project, and we want to create an instance in our scene. The code snippet below shows how this is done.

````cs

private void InstantiateBulletPrefab()
{
    // Note that "MyBulletPrefab" refers to the name and location of your prefab Asset
    Prefab myBulletPrefab = Asset.Load<Prefab>("MyBulletPrefab");
    var bullet = myBulletPrefab.Instantiate();

    // Change the X coordinate
    bullet.Transform.Position.X = 20.0f;
    SceneSystem.SceneInstance.Scene.Entities.Add(bullet);
}
````
