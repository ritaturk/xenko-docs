# Start scripting

In this section, you’ll learn the basics of [scripting](xref:scripting), how to create a script, how to use a script in your game, and how to launch your game.

## What is scripting

Scripting is an important part of creating a game. It helps you arrange your game events, respond to your inputs, control the movement and behavior of your [entities](xref:entity), and as a whole it helps to make your static game moving.

You can easily create your first game with Xenko assets. However, to move those [assets](xref:asset) and to make your game playing with actions and events, you need a script. In Xenko, you have to write all your scripts in C#. You can create a script for an asset in your game, attach that script to the asset, and then execute the game to make your game work in the expected way.

The following is a sample script of a game:

```
using System;
using System.Text;
using System.Threading.Tasks;
using SiliconStudio.Core.Mathematics;
using SiliconStudio.Xenko.Input;
using SiliconStudio.Xenko.Engine;

namespace MyGame
{
    public class BasicAsyncScript : AsyncScript
    {         
		public override async Task Execute() 
		{
            while(Game.IsRunning)
            {
				// Do some stuff every frame
                await Script.NextFrame();
            }
        }
     }
}
```
_Sample script_

This section includes the following pages:

* [Scripting in Xenko](scripting-in-xenko.md)
* [Create a script](create-a-script.md)
* [Use a script](use-a-script.md)
* [Launch your game](launch-your-game.md)

Start creating your own scripts for your assets. To learn more about scripting concepts, see [Scripting in Xenko](scripting-in-xenko.md).
