# Use a script

In this page, you’ll learn how to attach a script to an entity, how to test a script, and how to debug a script.

## Attach a script

You can attach a script to your entity either from the **Add component** section of [Game Studio](xref:game-studio) or through code.

**Attaching a script in Game Studio:**

1. Open your project in Game Studio.
2. Open your [scene](xref:scene), and then click the entity to which you want to attach a script.
3. Now drag and drop the script from the **Asset view** into the **Property grid** of the selected entity, in order to attach the script.
   
> **Note:** It is also possible to attach a script by using the **Add component** button in the **Property grid**.

**To attach a script through code:**

You can use code in Game Studio to attach a script to an entity.

1. In Visual studio, create a script called **BasicAsyncScript** and save it.

2. In order to attach the **BasicAsyncScript** script to an entity called **myEntity**, you can use the following code snippet:

```Code: 
// myEntity being an existing entity in the scene
myEntity.Add(new BasicAsyncScript());
```

## Test a script

You can test your script by running the game. Your script gets executed automatically when the entity to which you attached your script is loaded in the active scene.

**To test a script:**

1. Open your game in Game Studio.
2. Click ![Play icon](media/use-a-script-play-icon.png)to run your game.

If your code is working correctly, you'll see it's output in the running game. If something is not working correctly, you need to debug your script.

## Debugging a script

You need to debug your script if the script is not running properly or you are getting unexpected results.

**To debug a script:**

1. Open Visual Studio, and then open the script.

2. Press **F9** to add break points at the required place(s).

3. In Visual Studio, press **F5** or click the **Start** button to run the game in debug mode.

   Your game starts in a new window. In Visual Studio, on the script page, the first break-point highlights and stops the execution.
   
4. Verify the code.
5. Press **F10** (step over) if you want to execute the code line-by-line or press **F5** to continue code execution.

Now, you know how to attach, test, and debug a script. You can try to launch your game. For information on how to launch your game, see [Launch your game](launch-your-game.md).
