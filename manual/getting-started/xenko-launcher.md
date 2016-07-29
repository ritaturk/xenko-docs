# Xenko launcher

After you install Xenko, the first window that is displayed is the Xenko launcher. The launcher lets you manage and run the different versions that have been installed on your system. 

This page will show you the details of what you can do with the launcher.

![Xenko launcher interface](media/xenko-launcher-interface.png)

_Xenko launcher_

## Installing Xenko and starting the Game Studio

The launcher prompts you initially to the install latest version of Xenko as well as the Visual Studio plugin. Using this plugin, you can edit your [shaders](xref:shaders) directly from Visual Studio. This plugin provides the features of syntax highlighting, live-code-analysis with validation, error-checking, and navigation. It is not mandatory to install this plugin, however we recommend to install it.

You can start the active version of Game Studio by clicking the Start button. To change the active version, click a version in the **Switch/update** version section to make the selected version active.

![Xenko launcher: Start button](media/xenko-launcher-start-button.png)

_Start button of Xenko launcher_

## Version management

The Xenko launcher allows you to install mutliple versions of Xenko, and to switch between them. Versions might not be compatible with each other, and therefore the version of Xenko for which a project was developed, should be installed. This allows for projects that have been developed with different versions to keep working, without the need to upgrade them to a newer version.

If only the last number in the version number is changed, it means that it is a bug fix version only, and it does not contain changes that will break projects build on a previous version. It is safe and recommended to install these big fix versions. Note that these versions cannot be reverted.

After the Xenko installation has finished for the selected versions, click the required version. The version number of the selected version is displayed on the Start button. Now click the start button to launch the selected version.

![Various versions of Xenko](media/xenko-launcher-various versions.png)

_Various versions of Xenko_


For more details about the Xenko launcher see [Xenko launcher](/manual/xenko-launcher/).

Now, you’re ready to create your first project in Game Studio. For information on how to create a project, see [Create a project](create-project.md).
