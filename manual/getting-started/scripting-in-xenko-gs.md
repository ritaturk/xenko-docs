# Scripting in Xenko

In this page you will learn how to do scripting in Xenko, what types of scripts are used, how to script the public fields, and how the scripts are used in a project.

Scripting refers to adding a code to your game. After you create a game with some entities, initially all your entities will be static. To move your entity or to control their behavior, and to control and arrange events, you need to attach a code to your entity. 

>**Note:**  You need to create your scripts in C#.

## Script basics

A script can be attached to more than one entity. If you attach a script to more than one entity, then that creates more than one instance of the script. A script can be executed only when the entity to which the script is attached is added into the active scene.

A script can access engine services such as:
 * Content: content manager
 * Input 
 * Graphic device
 * Game
 * Log

For more information about Scripts, see [I will provide cross reference to the Reference Page.].

## Types of scripts

Scripts that you will be using for Xenko can be classified into: 
 * Startup
 * Synchronous 
 * Asynchronous 

### Startup script

This script is used to initialize an entity in the game, and is executed to perform loading or unloading of an entity in the game. For more information, see [Startup script].

### Synchronous script

This script loads sequentially and is executed sequentially. If a script is not executed, all the scripts that are in the sequence also get terminated. For more information and examples, see [Synchronous script].

### Asynchronous script

This script is not dependent on the execution of any other script. It can be executed randomly or with a combination of scripts without any dependency. For more information and examples, see [Asynchronous script].

## Script public fields

Xenko includes a set of public fields and properties. The value of any of these fields and properties can be set in Property grid in Xenko Studio.
For more information, see [Script public fields].

Now you know the scripting basics. You can start creating your script. For more information on how to create a script, see [Create a script].

