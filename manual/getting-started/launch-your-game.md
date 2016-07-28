# Launch your game

After your game is ready, you will be curious to see what your game looks like outside the Game studio. You can launch your game either on [Game Studio](xref:game-studio) or in Visual Studio.

In this page, you’ll learn various ways to launch your game.

Xenko has an integrated IDE which automatically opens your game in Visual Studio and allows you to write your script. This saves your time to open a project and create from scratch in Visual Studio.

## Run your Game in Game Studio

In Game Studio, you can run your game either through the Play icon or through Live Scripting.

### Run your game using the play icon

When you run your game for the first time, you can create a build and then run your game. This will help you to identify and fix any bug. You can also directly run your game.

**To run your game using the play icon:**

1. Click ![Build](media/launch-your-game-build-icon.png) to build your game or press **F6**.
   Your game build is created.

2. Click ![Play](media/launch-your-game-play-icon.png) to run or press **F5**.

   You can see the build status in the Output window. Your game starts in the selected platform.

### Run your game through the live scripting icon

Live scripting is a special mode where you can update your script while it is running.

**To run your game through the live scripting icon:**

1. Open your script in Visual Studio.
2. Click ![Live-scripting](media/launch-your-game-live-scripting-icon.png).

   >**Note:** Click the ![List](media/launch-your-game-platform-list.png) drop-down list to select the required platform. Currently Xenko supports Android and Windows.

## Run your Game in Visual Studio

You can run your game in Visual Studio. From Game Studio, you can initiate this.

**To run a game in Visual Studio:**

1. In Game Studio, click ![IDE](media/launch-your-game-ide-icon.png).

   Your game is opened in Visual Studio.

2. Click ![Start button](media/launch-your-game-start-button.png) or press **F5**.

   Your game starts in debug mode in Windows.
3. Press **Ctrl + F5**.

   Your game starts in run mode.

   >**Note:** By default, the Windows platform is selected. To run your game on other platforms, select the project assembly with the required platform. Right-click the required platform name, and then click **Set as Startup Project**. This sets the selected platform for your game. Press **F5** to run your game in the selected platform.

   ![Solution explorer](media/launch-your-game-select-platform.png)

   _Select Platform in Solution Explorer_

Now, you know how to launch your game in Game Studio and in Visual Studio.