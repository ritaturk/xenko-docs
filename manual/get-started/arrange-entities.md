# Arrange Entities

<span class="label label-doc-level">Beginner</span>
<span class="label label-doc-audience">Level Designer</span>

To build the levels of your game, you need to move, rotate, and resize the entities of your scene. Game studio provides you with gizmos to perform these operations.

This page will show you how to move, rotate, and resize your entities in a scene.


## Transformation Gizmos

Gizmos in Game Studio help you move, rotate, and resize your entities. You can find these gizmos at the top of the Scene Editor.

You can move an entity by first clicking the entity, and then through the Translation gizmo, dragging it along any of the X, Y, and Z axes. For example, to move an entity along the X axis, click the entity, and click and drag it along the X axis. You can also move the entity along two axes at the same time by clicking the center of the X, Y, and Z axes, and then dragging it in the required direction. Also, you can rotate and resize the entity using the Rotation and Scale gizmos, respectively.

Positioning the entities in your scene includes switching between gizmos, changing gizmo axis bases, doing multiple scales or translations, and snapping these operations.

You can see the following gizmos on the Scene Editor:
* Translation gizmo
* Rotation gizmo
* Scale gizmo

### Translation gizmo

The Translation gizmo ![Translation gizmo](media/manage-entities-in-scene-translation-gizmo.png) changes the position of the selected entity. The following video shows how you can translate an entity along one axis, a plane (2 axes) or freely in 3D.

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

### Scaling and translation in all 3 dimensions

You can perform a translation over all 3 axes by clicking the center of the Translation gizmo ![Translation gizmo](media/manage-entities-in-scene-translation-gizmo.png).

**To perform translation over 3 axes:**

1. Select an entity.
2. Select the Translation gizmo.
3. Left-click and drag the center of the Translation gizmo to move the entity over all 3 axes.

You can perform multiple scaling over all 3 axes by clicking the center of the Scale gizmo.

**To perform multiple scaling over 3 axes:**

1. Select an entity.
2. Select the Scale gizmo.
3. Left-click and drag the center of the Scale gizmo to scale the entity in all 3 axes.

## Switching between gizmos

To switch between the gizmos, you can either click on the respective buttons, or use keyboard shortcuts to change between them. Before using the keyboard shortcuts, you must first make the Scene editor active, by clicking anywhere in the Scene Editor. Then, you can switch between Translation, Rotation and Scaling by:

* Pressing the Spacebar - this rotates between the Translate, Rotate, and Scale gizmos.
* Press the **W** key to switch to the Translation gizmo.
* Press the **E** key to switch to the Rotation gizmo.
* Press the **R** key to switch to the Scale gizmo.

## Change gizmo coordinate system

In Game Studio, you can select in which coordinate system the gizmo operates. The following table displays the gizmo axis bases and their functions:

| Gizmo axis base | Function |
| ------  |  ------  |
| ![World space coordinates](media/manage-entities-in-scene-wsc.png) | Uses the world coordinate system for transformations. The X, Y, and Z axes are the same for every entity. |
| ![Object space coordinates](media/manage-entities-in-scene-osc.png)  | Uses the local coordinate system for transformations. The axes are oriented in the same direction as the selected entity. |
| ![Camera space coordinates](media/manage-entities-in-scene-csc.png) | Uses the current camera coordinate system for transformations. The axes are oriented in the same direction as the editor camera. |


**To change the axis base for a gizmo:**

1. Select an entity.
2. Click the button representing the required coordinate system.
   
> [!WARNING] 
> The Translation gizmo and the Rotation gizmo can use all coordinate systems. 
> However, the Scale gizmo can only use the local coordinate system.

## Snapping gizmo actions

While using the gizmos, you can snap the action you perform by using the Snapping tool. This means that the amount of rotation / translation / scaling is snapped to the closest multiple of the number you specify. I.e.: if you set the snap to grid value to 22.5 for rotating, your rotation action will be a multiple of 22.5: 0, 22.5, 45, 67.5, 90 etc.

Based on the gizmo you selected, the icon on the Snapping tool changes. 

   ![Snap translations](media/manage-entities-in-scene-snap-translation.png)
   
   _Snap translations to value 1_
   
   ![Snap rotations](media/manage-entities-in-scene-snap-rotation.png)
   
   _Snap rotations to value 22.5_
   
   ![Snap scale](media/manage-entities-in-scene-snap-scale.png)
   
   _Snap scale to factor 1.1_

Now you know how to arrange the entities in your scene. Next you will learn how to move inside the scene editor.
See [Navigate inside the scene editor](navigate-in-the-editor.md).