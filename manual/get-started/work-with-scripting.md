# Scripting in Xenko

You are aware of scripting basics. In this page you will learn the details about scripting, such as, reason for scripting, how we can use a script in a game, and finally how can you see the result of your script.

In Xenko, a game may be very simple or complex. There should be a script, which helps the events of the game to arrange in an order, responds to input from the player, creates effects to the graphics, control your entities movement and behavior, and many actions.

In this page, you will learn:
 * Basics of Scripting
 * Types of Scripts
 * Scripting public fields

## Basics of Scripting

### Script

A script is a small unit of code, which can be attached to an asset or entity of a game. A script may be simple, small code or a complex code, but it is used to control an asset or entity’s movement. Without a script your game is a static image.

### Uses of Script

A game has a container called a scene, which has objects called assets or entities (we refer to an asset as an entity), models, and components. It contains series of events where the objects move around your game, respond, and change with various effects. All this is possible using a script.

With the help of script you can:
 * Arrange events of your game in a sequence.
 * Move your objects and animate them.
 * Communicate with user and respond.
 * Control the movement of objects.
 * Add sounds, visual effects and control them.


### Script and entity

A script can be attached to more than one entity and more than one script can be attached to a single entity. If more than one entity requires same set of actions to be done, then you can create a script which can be attached to those entities. If you attach a script to more than one entity, then that creates more than one instance of the script for that entity.

If a script has more than one instance, in that case, to avoid confusion of blocking, you can set priority value to such scripts to run accordingly. The priority values of the scripts can be set in Priority grid of Xenko Studio.

### Executing a script

Now, you have created a script and attached it to an entity. But to execute, the entity to which the script is attached should be added to the active scene. Now you are ready to execute your script.
Execute your game, to execute your game, press the play button on the tool bar or press F5. The game executes and plays the entity to which your script is attached.

### Scripts and services

Scripts also access various services in Xenko. Services are the ready If a graphic is to be animated using a script, the scripts uses an engine service called Graphic Device, which contains all the graphical effects.

The basic services that can be accessed by scripts are:
 * Content: content manager
 * Input 
 * Graphic device
 * Game
 * Log

## Types of scripts

Xenko uses different types of scripts: Startup script, Synchronous script, Asynchronous script.

### Startup script

This script is used to initialize an entity in the game, and is executed to perform loading or unloading of an entity in the game.

Following methods are used in Startup script:

List all the methods used with example.

Examples:

List examples of startup script with description.

### Synchronous script

This script loads sequentially and is executed sequentially. If a script is not executed, all the scripts that are in the sequence also get terminated.

Following are the methods used in this script:

List all the methods used with examples.

Examples:

List examples with description.

### Asynchronous script

This script is not dependent on the execution of any other script. It can be executed randomly or with a combination of scripts without any dependency.

Following are the methods used in this script:

List all the methods used with examples.

Examples:

List examples with description.

## Script public fields

Xenko includes a set of public fields and properties. The value of these fields and properties can be set in Property grid in Game Studio.

Then, explanation about property grid and how can we set the public fields in the property grid with images.
Information about can we ignore using public fields? How?

Example of pubic fields
Image displaying public field and its equivalent in the property grid.
