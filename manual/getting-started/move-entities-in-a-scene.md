# Move entities in a scene

In this topic, you will learn how to move entities in a scene.

To place an entity in a scene, you need to move the entity by changing its position and orientation. You can also resize the entity. You can use gizmos to perform these functions.

## Gizmo

Gizmos in Xenko Studio help you move, rotate, and resize your entities effectively. These gizmos have the following types and functions:

   _Gizmos and their functions_

| Gizmo  | Function  |
| ------ | ------    |
| ![Translation gizmo](media/move-entities-in-scene-translation-gizmo.png) | Translation gizmo, changes the position of the selected entity. |
| ![Rotation gizmo](media/move-entities-in-scene-rotation-gizmo.png) | Rotation gizmo, changes the orientation of the selected  entity.|
| ![Scale gizmo](media/move-entities-in-scene-scale-gizmo.png) | Scale gizmo, resizes the selected entity. |

## Switch between gizmos

You can switch between Translation, Rotation, and Scale gizmos through simple clicks.

To switch between the gizmos, you must first click anywhere in the Scene Editor. Then, you can:

* Click a gizmo icon to switch to that particular gizmo.
  
  or
 
* Press the Spacebar.

  or

* Press the **W** key to switch to the Translation gizmo
* Press the **E** key to switch to the Rotation gizmo
* Press the **R** key to switch to the Scale gizmo

## Change gizmo axis bases

Xenko Studio provides the following gizmo axis bases:

   _Gizmo axis bases and their functions_

| Gizmo axis base | Function |
| ------  |  ------  |
| ![World space coordinates](media/move-entities-in-scene-wsc.png) | Uses the world coordinates for transformations. The X, Y, and Z axes are the same for every entity. |
| ![Object space coordinates](media/move-entities-in-scene-osc.png)  | Uses the local coordinates for transformations. The axes are oriented in the same direction as the selected entity. |
| ![Camera space coordinates](media/move-entities-in-scene-csc.png) | Uses the current camera projection coordinates for transformations. The axes are oriented in the same direction as the editor camera. |

To change the axis base for a gizmo:

1. Select an entity.
2. Click a gizmo axis base button.

>**Note:** The Translation gizmo and the Rotation gizmo can use all the three axis bases. However, the Scale gizmo can use only the axis base that uses the local coordinates for transformations.

## Multiple scale or translation

You can perform multiple translations by clicking the center of the Translation gizmo.

To perform multiple translations:

1. Select an entity.
2. Select the Translation gizmo.
3. Click the center of the Translation gizmo.
   You can now drag the entity horizontally, vertically, and diagonally.

You can perform multiple scales by clicking the center of the Scale gizmo.

To perform multiple scales:

1. Select an entity.
2. Select the Scale gizmo.
3. Click the center of the Scale gizmo.
   You can now increase the size of the entity proportionally.

## Snap entities to the grid

While using the gizmos, you can snap an entity to the grid by using the Snapping tool. Based on the gizmo you select, the icon on the Snapping tool changes.

   ![Snap translations](media/move-entities-in-scene-snap-translation.png)
   
   _Snap translations to value 1_
   
   ![Snap rotations](media/move-entities-in-scene-snap-rotation.png)
   
   _Snap rotations to value 0.5_
   
   ![Snap scale](media/move-entities-in-scene-snap-scale.png)
   
   _Snap scale to factor 1.1_

To snap an entity to the grid:

1. Select an entity.
2. Select a gizmo.
3. Select the Snapping tool and enter a value in the tool.
4. Drag the entity.

   The entity snaps as per the value that you specified.

Thus, you can easily move the entities in a scene by using gizmos.

The next step is to animate the entities in your scene. To do this, you need to use scripts. For information about using scripts, see [Scripting in Xenko](http://doc.xenko.com/latest/manual/getting-started/howto-use-scripts.html).
