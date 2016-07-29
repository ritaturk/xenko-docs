# Manage entities in a scene

To build the levels of your game, you need to move, rotate, and resize the entities of your scene. Game studio provides you with gizmos to perform these operations.

This page will show you how to move, rotate, and resize your entities in a scene.

### Focus on an entity

While editing the properties of a specific entity, you may need to view it in a full screen mode so that you can properly see all the subtle changes that you have made to that entity. To do this, you can press the **F** key after selecting the entity. This action automatically zooms on the entity and adjusts the position of the editor camera.

Alternatively, you can click ![Magnifier icon](media/navigate-in-a-scene-magnifier-icon.png) from the Scene explorer view to focus on the entity without having to select it first.

The following animations display focusing on an entity using the Magnifier icon and using the **F** key, respectively.

<div class="video_container">
  <div class="video_container_left">
   ![Switch Projection Mode](media/navigate-in-scene-focus-on-entity-using-magnifier-icon.gif)
   </video>
   <div class="video_container_content">_Focus on an entity using Magnifier icon_</div>
   </div>
   <div class="video_container_right">
   ![Switch Projection Mode](media/navigate-in-scene-focus-on-entity-using-f-key.gif)
   </video>
   <div class="video_container_content">_Focus on an entity using F key_</div>
   </div>
</div>

<div style="clear: both;"></div>

## Transformation Gizmos

Gizmos in Game Studio help you move, rotate, and resize your entities effectively. They are present at the top of the Scene Editor.

You can move an entity by first clicking the entity, and then through the Translation gizmo, dragging it along any of the X, Y, and Z axes. For example, to move an entity along the X axis, click the entity, and click and drag it along the X axis. You can also move the entity along two axes at the same time by clicking the center of the X, Y, and Z axes, and then dragging it in the required direction. Also, you can rotate and resize the entity using the Rotation and Scale gizmos, respectively.

Managing the entities in your scene includes switching between gizmos, changing gizmo axis bases, doing multiple scales or translations, and snapping the entities to the grid.

You can see the following gizmos on the Scene Editor:
* [Translation](xref:translation) gizmo
* [Rotation](xref:rotation) gizmo
* [Scale](xref:scale) gizmo

### Translation gizmo

The Translation gizmo ![Translation gizmo](media/manage-entities-in-scene-translation-gizmo.png) changes the position of the selected entity. The following video shows how you can translate an entity along one axis, a plane, freely in 3D.

<video controls autoplay loop height="480" width="640">
                <source src="media/manage-entities-in-scene-translation-gizmo.mp4" type="video/mp4">
</video>

_Video: Translate an entity_

### Rotation gizmo

The Rotation gizmo ![Rotation gizmo](media/manage-entities-in-scene-rotation-gizmo.png) changes the orientation of the selected entity. The following video shows how you can rotate an entity along one axis.

<video controls autoplay loop height="480" width="640">
                <source src="media/manage-entities-in-scene-rotation-gizmo.mp4" type="video/mp4">
</video>

_Video: Rotate an entity_

### Scale gizmo

The Scale gizmo ![Scale gizmo](media/manage-entities-in-scene-scale-gizmo.png) resizes the selected entity. The following video shows how you can scale an entity along one axis and along all three axes.

<video controls autoplay loop height="480" width="640">
                <source src="media/manage-entities-in-scene-scale-gizmo.mp4" type="video/mp4">
</video>

_Video: Scale an entity_

## Switch between gizmos

You can switch between Translation, Rotation, and Scale gizmos through simple clicks.

To switch between the gizmos, you must first click anywhere in the Scene Editor. Then, you can switch between Translation, Rotation and Scaling by:

* Clicking a gizmo icon to switch to that particular gizmo.
* Pressing the Spacebar
* Press the **W** key to switch to the Translation gizmo
* Press the **E** key to switch to the Rotation gizmo
* Press the **R** key to switch to the Scale gizmo

## Change gizmo coordinate system

In Game Studio, you can select in which coordinate system the gizmo operates. The following table displays the gizmo axis bases and their functions:

| Gizmo axis base | Function |
| ------  |  ------  |
| ![World space coordinates](media/manage-entities-in-scene-wsc.png) | Uses the world coordinates for transformations. The X, Y, and Z axes are the same for every entity. |
| ![Object space coordinates](media/manage-entities-in-scene-osc.png)  | Uses the local coordinates for transformations. The axes are oriented in the same direction as the selected entity. |
| ![Camera space coordinates](media/manage-entities-in-scene-csc.png) | Uses the current camera projection coordinates for transformations. The axes are oriented in the same direction as the editor camera. |


**To change the axis base for a gizmo:**

1. Select an entity.
2. Click the button representing the required coordinate system.
   
   The axis base for a gizmo is changed.

>**Note:** The Translation gizmo and the Rotation gizmo can use all coordinate systems. However, the Scale gizmo can only use the local coordinate system.

## Scaling and translating in all 3 dimensions

You can perform a translation over all 3 axes by clicking the center of the Translation gizmo ![Translation gizmo](media/manage-entities-in-scene-translation-gizmo.png).

**To perform translation over 3 axes:**

1. Select an entity.
2. Select the Translation gizmo.
3. Click the center of the Translation gizmo.
   You can now drag the entity horizontally, vertically, and diagonally.

You can perform multiple scaling over all 3 axes by clicking the center of the Scale gizmo.

**To perform multiple scaling over 3 axes:**

1. Select an entity.
2. Select the Scale gizmo.
3. Click the center of the Scale gizmo.
   You can now increase the size of the entity proportionally.

## Snapping gizmo actions

While using the gizmos, you can snap the action you perform by using the Snapping tool. This means that the amount of rotation / translation / scaling is snapped to the closest multiple of the number you specify. I.e.: if you set the snap to grid value to 22.5 for rotating, your rotation action will be a multiple of 22.5: 0, 22.5, 45, 67.5, 90 etc.

Based on the gizmo you selected, the icon on the Snapping tool changes. 

   ![Snap translations](media/manage-entities-in-scene-snap-translation.png)
   
   _Snap translations to value 1_
   
   ![Snap rotations](media/manage-entities-in-scene-snap-rotation.png)
   
   _Snap rotations to value 22.5_
   
   ![Snap scale](media/manage-entities-in-scene-snap-scale.png)
   
   _Snap scale to factor 1.1_


The next step is to make your scene more dynamic. To do this, you need to use scripts. For information about using scripts, see [Scripting in Xenko](scripting-in-xenko.md).
