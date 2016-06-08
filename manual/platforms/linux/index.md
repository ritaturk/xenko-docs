# How to develop a project and target Linux?

##Creation and Compilation

Create a project in GameStudio and make sure to choose Linux as a platform choice. At this point you need to choose if you want to run your program against Mono (default) or CoreCLR. You can choose this in the properties of your solutions by using either _Release_ or _Debug_ for Mono and _CoreCLR_Release_ or _CoreCLR_Debug_ for CoreCLR.

Once this is done, proceed as usual to compile this project in Visual Studio or from the command line by using MSBuild (`msbuild your_solution.sln /p:Platform=Linux /p:Configuration="YourChosenConfigurationHere"`).

##Copying Files over

Depending on your Configuration (_Release_ vs _Debug_, and _CoreCLR_Release_ and _CoreCLR_Debug_), you will find all the files required to run on Linux in **Bin\Linux\YourChosenConfigurationHere**). Copy those files over to your Linux environment.

##Setting up the environment for Linux

You are almost ready to run your program on Linux. The only remaining step is to map all the shared libraries (i.e. .so and .dll) to your system. Depending if you are running Mono or CoreCLR, the required steps are different.

###Mono

_To be completed_

###CoreCLR

We provide a packaged CoreCLR, assuming you have expanded it in "~/CoreCLR" and that for all shared libraries you are using you have created a link to their Linux counterpart, you can simply run

`~/CoreCLR/corerun -c ~/CoreCLR yourExecutable.exe`
