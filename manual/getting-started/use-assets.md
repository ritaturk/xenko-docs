# Use Assets

This page will show you how to use your assets once you've created them.

## Referencing Assets

Some Assets require a reference to other Assets. Examples are:

* A (procedural) model Asset can have a reference to a ***Material***
* An animation Asset uses a reference to a ***Model*** Asset, and a reference to a ***Skeleton*** Asset

By clicking these Assets, note that you can select an Asset to reference in the Property grid. These references typically have specific names to indicate what the reference is for, such as ***Material***, ***Model*** or ***Skeleton***.

## Loading Assets from code

It is also possible to load Assets from code. The code below shows you an example of this:

```cs

public class AddAssetScript : StartupScript
{
	public override void Start()
	{
		// URL should be replaced with the URL to the Model you'd like to add to your scene
		Model model = Content.Load<Model>("URL");

		// The entity's initial position
		Vector3 position = new Vector3(0.0f, 0.0f, 0.0f);

		// Now create a new entity to add to our current Scene
		Entity entity = new Entity(position, "Entity Added by Script")
		{
			new ModelComponent { Model = model }
		};

		SceneSystem.SceneInstance.Scene.Entities.Add(entity);
	}
}

```

Be sure to properly include the Asset as described in the previous chapter, by marking the Asset to be included in the ***Asset view***. Also make sure to add the Script as a component to an Entity in the Scene in order to get executed.

Next, you'll learn how to create a Scene in Game Studio, see [Introduction to scenes](introduction-to-scenes.md)
