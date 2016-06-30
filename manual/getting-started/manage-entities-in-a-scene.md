# Manage entities in a scene

To build the levels of your game, you need to move, rotate, and resize the entities of your scene. Xenko provides you gizmos to perform all these functions.

In this page, you’ll learn how to move, rotate, and resize your entities in a scene.

## Transformation Gizmos

Gizmos in Game Studio help you move, rotate, and resize your entities effectively. They are present at the top of the Scene Editor.

You can move an entity by first clicking the entity, and then through the Translation gizmo, dragging it along any of the X, Y, and Z axes. For example, to move an entity along the X axis, click the entity, and drag it along the X axis. You can also move the entity along two axes at the same time by clicking the center of the X, Y, and Z axes, and then dragging it in the required direction. Also, you can rotate and resize the entity using the Rotation and Scale gizmos, respectively.

Managing the entities in your scene includes switching between gizmos, changing gizmo axis bases, doing multiple scales or translations, and snapping the entities to the grid.

You can see the following gizmos on the Scene Editor:
* [Translation](xref:translation) gizmo
* [Rotation](xref:rotation) gizmo
* [Scale](xref:scale) gizmo

### Translation gizmo

The Translation gizmo ![Translation gizmo](media/manage-entities-in-scene-translation-gizmo.png) changes the position of the selected entity. The following video shows how you can translate an entity along one axis, a plane, freely in 3D.

<video controls poster="media/xenko-poster-image-640by480.png" height="480" width="640">
                <source src="media/manage-entities-in-scene-translation-gizmo.mp4" type="video/mp4">
</video>

_Video: Translate an entity_

### Rotation gizmo

The Rotation gizmo ![Rotation gizmo](media/manage-entities-in-scene-rotation-gizmo.png) changes the orientation of the selected entity. The following video shows how you can rotate an entity along one axis.

<video controls poster="media/xenko-poster-image-640by480.png" height="480" width="640">
                <source src="media/manage-entities-in-scene-rotation-gizmo.mp4" type="video/mp4">
</video>

_Video: Rotate an entity_

### Scale gizmo

The Scale gizmo ![Scale gizmo](media/manage-entities-in-scene-scale-gizmo.png) resizes the selected entity. The following video shows how you can scale an entity along one axis and along all three axes.

<video controls poster="media/xenko-poster-image-640by480.png" height="480" width="640">
                <source src="media/manage-entities-in-scene-scale-gizmo.mp4" type="video/mp4">
</video>

_Video: Scale an entity_

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

In Game Studio, gizmo axis bases are present at the top of the Scene Editor.

The following table displays the gizmo axis bases and their functions:

| Gizmo axis base | Function |
| ------  |  ------  |
| ![World space coordinates](media/manage-entities-in-scene-wsc.png) | Uses the world coordinates for transformations. The X, Y, and Z axes are the same for every entity. |
| ![Object space coordinates](media/manage-entities-in-scene-osc.png)  | Uses the local coordinates for transformations. The axes are oriented in the same direction as the selected entity. |
| ![Camera space coordinates](media/manage-entities-in-scene-csc.png) | Uses the current camera projection coordinates for transformations. The axes are oriented in the same direction as the editor camera. |


**To change the axis base for a gizmo:**

1. Select an entity.
2. Click a gizmo axis base button.
   
   The axis base for a gizmo is changed.

>**Note:** The Translation gizmo and the Rotation gizmo can use all the three axis bases. However, the Scale gizmo can use only the axis base that uses the local coordinates for transformations.

## Multiple scales or translations

You can perform multiple translations by clicking the center of the Translation gizmo ![Translation gizmo](media/manage-entities-in-scene-translation-gizmo.png).

**To perform multiple translations:**

1. Select an entity.
2. Select the Translation gizmo.
3. Click the center of the Translation gizmo.
   You can now drag the entity horizontally, vertically, and diagonally.

You can perform multiple scales by clicking the center of the Scale gizmo.

**To perform multiple scales:**

1. Select an entity.
2. Select the Scale gizmo.
3. Click the center of the Scale gizmo.
   You can now increase the size of the entity proportionally.

## Snap entities to the grid

While using the gizmos, you can snap an entity to the grid by using the Snapping tool. Based on the gizmo you selected, the icon on the Snapping tool changes.

   ![Snap translations](media/manage-entities-in-scene-snap-translation.png)
   
   _Snap translations to value 1_
   
   ![Snap rotations](media/manage-entities-in-scene-snap-rotation.png)
   
   _Snap rotations to value 22.5_
   
   ![Snap scale](media/manage-entities-in-scene-snap-scale.png)
   
   _Snap scale to factor 1.1_

**To snap an entity to the grid:**

1. Select an entity.
2. Select a gizmo.
3. Select the Snapping tool and enter a value in the tool.
4. Drag the entity.

   The entity snaps as per the value that you specified.

Thus, you can easily move, rotate, and resize the entities in a scene by using gizmos.

The next step is to animate the entities in your scene. To do this, you need to use scripts. For information about using scripts, see [Scripting in Xenko](scripting-in-xenko.md).