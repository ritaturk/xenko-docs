# Project structure

This page will show how Xenko organizes its project structure. Understanding the Xenko project structure is essential for knowing where to place and find files, collaboration and scaling your project.

#Packages

Xenko organizes its projects in packages. A package is an aggregation of:

* Assets: An asset is a representation of an object or resource inside the editor, see [Introduction to Assets](introduction-to-assets.md) for more information.
* Resources: Resources refers to raw files such as images, textures, and audio, that are embedded in the package.
* Scripts: Scripts contain logic that make your game dynamic, see [Scripting in Xenko](scripting-in-xenko.md) for more information.

A package can depend on other packages. A package and all its dependencies make up an independent unit that can be reused in other games or applications.

## Package directory structure

In Xenko, a package is a collection of Assets, Resources, Scripts. In Game Studio, the Solution explorer section displays the folder hierarchy of your game, which matches the package folder structure.

For example, for a project named 'MyGame', the directory structure is as follows:

![Xenko Sample Directory Structure](media/sample-project-directory-structure.png)

1. **Assets** Contains all the assets used in the project. (Models, materials, etc.)
2. **Bin** Contains all the binariesof yours game on the respective platform. A subdirectory for each platform is created, and contains the files needed to run on that platform.
3. **MyGame.Game** Contains all the game specific source code.
4. **MyGame._Platform_** Contains all the platform specific source code. A subdirectory containing the platform name is created for every selected platform. (e.g. MyGame.Linux, MyGame.Windows etc.).
5. **Resources** Contains all files containing the raw information that needs to be embedded in the game, like: images, audio, FBX files, XML files, etc.

Now, as you know how to organize your project, you can start creating your own assets, see [Introduction to Assets](introduction-to-assets.md).
