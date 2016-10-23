## What are conversion references?
Outfit Studio comes with so called conversion references, which consist of one or more **sliders** that can morph a mesh from one shape to another.

The mesh provided with the conversion reference is the **reference shape**.

Other meshes loaded into Outfit Studio can be conformed to these sliders, so that they will morph along with the reference shape.

One example where this can be made use of, is to convert an outfit **from one body type to another** (slider value 0% -> 100%).

## Loading up references
To load a conversion reference, choose the **File -> Load Reference** menu item and select your reference in the template drop down list.

[[Templates|Reference Templates]] are defined in the RefTemplates.xml file and point to a specific installed project and shape to load. Click the link if you want to know how to add new templates to the list.

If your conversion reference is not in the template list, you can also **manually choose the project file** (.osp) to use as the reference. Only one shape can be the reference at the same time.

_NIF files can be loaded as references as well, but they don't have sliders, so they're usually not of any use for shape conversions._

## The conversion reference you need doesn't exist?
If there is no conversion reference that directly morphs from your source shape to the required target shape, then you can simply go through the process multiple times by converting **from shape A to B first**, and afterwards **from shape B to your target shape C**.

This effectively uses shape B as a bridge to get to what you need, no matter its shape.

Examples of shape B as a bridge for conversion:
* A -> **B** -> C
* C -> **B** -> A
* B -> **B** -> D

## Step-by-step example
The following is a guide on how to **convert meshes from one shape to another** using a conversion reference.

If you want to create a BodySlide conversion (with slider compatibility) as well, follow the guide for that after you're done with this one. The reason being that you need the outfit to **fit the base shape first** before you can add the sliders.

1. Create a new project in Outfit Studio using the **New Project** button or menu item.

2. Select the **reference template** you need from the drop down list and click next.  
_Example: "Vanilla to CBBE"_

3. Choose the **file of the outfit/mesh** you want to convert and click next.
_Example: "outfit.nif"_

    **For Skyrim:** The high weight variants you need have the "_1" suffix attached to their file name. Other Bethesda games, such as Fallout 3 or Fallout 4, do not have weight variants.

4. **Delete the duplicate body shape** that was loaded together with the outfit file, if there is one. To do this, select the shape and press the DEL key or right-click it and choose "Delete Shape". If you don't do this, you might have two exported body shapes in one file later on.

5.** Conform the outfit shapes** to the sliders of the conversion reference. To do this, use the **Slider -> Conform All** menu item. It doesn't matter what shape you have selected here, as everything will be conformed.

6. Change the slider with the morph that you need **to 100%** and use the **Slider -> Set Base Shape** function. This will make the 100% value of the slider the **default shape of the mesh**. Any clipping here is normal and will be fixed later on!

7. Use the **File -> Load Reference** menu item and select the template/project (or .nif file) of the target body/mesh you have been converting to. This will load the mesh you actually want to use in-game.  
_Example: "CBBE Body" or "FemaleBody.nif"_

8. Now you might have to **fix a bit of clipping** here and there using the brush tools that Outfit Studio provides. Select the shape of the outfit you want to adjust, fix the clipping and do whatever tweaks you like. This is **editing the base shapes** of the meshes, not any slider morphs.

    Read up on the [[brushes page|Brushes]] for more info about them.

9. Next up, you have to **copy the bone weights** from your reference to your outfit/mesh, so that it will move along correctly with animations in-game. To do that, **multi-select** all of the outfit shapes in the list and choose **Copy Bone Weights** after a right-click.

10. Export the finished conversion using **File -> Export -> Export NIF With Reference**!

    **For Skyrim:** Replace the high weight variant of the outfit you converted with this file (**_1.nif**). Then, **repeat the entire process** with a different reference to target the low weight variant as well, but do NOT copy the bone weights a second time (**_0.nif**).