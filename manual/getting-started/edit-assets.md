# Edit assets

After you add an asset to your game project, you may need to make some changes to the asset in order to make it suitable to your game environment.

In this page, you’ll learn how to edit your game assets. As an example, you’ll change the color of a Sphere [Procedural Model](xref:procedural-model).

In Game Studio, the **Property grid** section includes the required options to edit your assets.

**To change the color of the Sphere Procedural Model:**

 1. On the **Asset view** tab, select the Sphere Material.
 
	![Sphere Material on the Asset view tab](media/edit-asset-sphere-material-asset-view-tab.png)

	_Sphere Material on the Asset view tab_
	
	The **Property grid** section shows the properties of the selected material.

 2. In the **Property grid** section, find the **Diffuse** property under **Shading**, and then click the **Diffuse Map** drop-down arrow.
 
	![Diffuse Map in Shading](media/edit-asset-diffuse-map-shading.png)
 
	_Diffuse Map in Shading_
	
	By default, [Diffuse Map](xref:diffuse-map) appears with Texture mapping. However, you can change the mapping to Vertex Stream, Binary Operator, Color, Float4, and Shader as per your need. Based on your selection in the Diffuse Map, other properties of shading change. For example, if you select the Color option in Diffuse Map, you can select a color using the color-picker or color-palette or you can directly enter the hexadecimal code for a color.
 
	![Color picker and Palette](media/edit-asset-color-picker-palette-diffuse.png)	
 
 	_Color picker and Palette_
	
 3. Click the drop-down arrow on the right of the diffuse map and select the **Color** property.
	
	The **Color picker** and **Palette** tabs are displayed.

 4. Click the **Color picker** and select a red hue color or type the hexadecimal value.
	
	After you set the color for the material, the color of the asset changes.
	
	![Asset appears in new color](media/edit-asset-color-change-selected-asset.png)

	_Asset appears in new color_
 
	The color of the Sphere Procedural Model changes to red.
	
	
To remove the references that have been applied to the Procedural Model, select the model for which you want to remove the references, and then click ![clear icon](media/edit-asset-clear-reference.png). This action directly removes all references that are applied to the model.

![Clear reference in Property grid](media/edit-asset-clear-reference-property-grid.png)
 
_Clear reference in Property grid_
	
You’ve learned how to edit an asset. You are now ready to create the first scene of your game project. For information on creating a scene, see [Scene creation](scene-creation.md).