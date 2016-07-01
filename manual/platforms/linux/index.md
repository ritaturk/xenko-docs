# Xenko On Linux

## Setup

Make sure to first follow the [requirements and setup instruction](setup.md)

##Creating Your First Linux Game

Create a project in GameStudio and make sure to choose Linux as a platform choice. At this point you need to choose if you want to run your program against Mono (default) or CoreCLR. You can choose this in the properties of your solutions by using either _Release_ or _Debug_ for Mono and _CoreCLR_Release_ or _CoreCLR_Debug_ for CoreCLR.

Once this is done, proceed as usual to compile this project in Visual Studio or from the command line by using MSBuild (`msbuild your_solution.sln /p:Platform=Linux /p:Configuration="YourChosenConfigurationHere"`).
