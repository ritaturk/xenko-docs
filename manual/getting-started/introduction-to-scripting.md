# Introduction to scripting

This section will discuss the following subjects:

* [Scripting in Xenko](scripting-in-xenko.md) - Basic concepts about scripting in Xenko.
* [Create a script](create-a-script.md) - How to create a script in both Visual Studio and Game Studio
* [Use a script](use-a-script.md) - How to attach and test scripts

<small>For more advanced topics, please refer to [Scripting](/manual/game-studio/scripting.md) in the Game Studio documentation</small>

## What is scripting

Scripting is an important part of game creation. Scripting, for example helps you handle game events, respond to user inputs, helps you control the movement and behavior of your Entities, and as a whole it helps to make your static game interactive.

All scripting in Xenko is done in C#, therefore you can use the C# programming reference, to find out about language specific information you might need.

Below you'll see an example of a C# script for Xenko.

```cs
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

Let's continue to learn more about basic scripting concepts, see [Scripting in Xenko](scripting-in-xenko.md).
