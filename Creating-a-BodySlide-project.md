## What are BodySlide projects?
BodySlide projects are created in Outfit Studio and can contain an outfit or body with **sliders for customization**. They can be selected from a list and the final result can be built straight into the data folder of your game.

![Project](http://i.imgur.com/fW6FuGO.png)

That means, we need to **create the slider data** for your outfit, so that it can morph together with the body/reference. Only after that you will be able to apply your custom presets in the BodySlide part of the program.

The outfit you're intending to use **has to be converted to the base shape** of the body/reference already, such as the base shape of the CBBE body for the specific game. If it is not, please follow the [[other guides|Guides and Documentation]] to do that first!

## How do I share project files with others?
After you're done creating your BodySlide project following the instructions below, there should be **multiple new files** in your BodySlide folder with the names you provided **in the save dialog**.

Projects consist of the following:
* **.osp** files from the **SliderSets** folder, which can contain multiple of your projects at once.
* **.osd** files from the **ShapeData/YourProject** folder, which contain the slider data for all meshes of a specific project.
* **.nif** files from the **ShapeData/YourProject** folder, which are the meshes themselves.
* (optionally) **.xml** files from the **SliderGroups** folder.

Make sure to provide them with the correct folder structures, and you and your users should be good to go.

![Folder Structure](http://i.imgur.com/Wt0bif1.png)

## Step-by-step example
This guide explains how to create such a project, so that you can make any outfit that you previously made or downloaded compatible with **existing sliders**.

1. Create a new project in Outfit Studio using the **New Project** button or menu item.  
![New Project](http://i.imgur.com/KxNNU2K.png)

2. Select the **[[conversion reference|Conversion references and using them]], [[template|Reference Templates]]** or project file that contains the sliders you need from the list or file browser and click next.  
_Example: "CBBE Body"_

3. Choose the **file of the outfit/mesh** you want to convert and click next.  
_Example: "outfit.nif"_

    **For Skyrim:** The high weight variants you need have the "_1" suffix attached to their file name. Other Bethesda games, such as Fallout 3 or Fallout 4, do not have weight variants.

    ![Outfit](http://i.imgur.com/GC8l0Ar.png)

4. **Delete the duplicate body shape** that was loaded together with the outfit file, if there is one. To do this, select the shape and press the DEL key or right-click it and choose "Delete Shape". If you don't do this, you might have two exported body shapes in one file later on.

5. Now you might have to **fix a bit of clipping** here and there using the brush tools that Outfit Studio provides. Select the shape of the outfit you want to adjust, fix the clipping and do whatever tweaks you like. This is **editing the base shapes** of the meshes, not any slider morphs.

    Read up on the [[brushes page|Brushes]] for more info about them.

6. **Conform the outfit shapes** to the sliders of the conversion reference.  
To do this, use the **Slider -> Conform All** menu item. It doesn't matter what shape you have selected here, as everything will be conformed.

    [![Conform All](http://i.imgur.com/sf1FvMZm.png)](http://i.imgur.com/sf1FvMZ.png)

7. (optional but recommended) **Check all sliders for clipping** and fix it using the brushes.  
To do that, select the shape that needs fixing, click the edit button next to the slider that requires tweaks and brush on.

    * It is only possible to edit one slider at the same time, but you can edit that one for multiple shapes at once.
    * Edit the outfit shapes, not the body/reference!
    * Note that the look of more extreme sliders might be hard to perfect sometimes.

    ![Edit Slider](http://i.imgur.com/ONVygUd.png)

8. Next up, you have to **copy the bone weights** from your reference to your outfit, so that it will move along correctly with animations in-game. To do that, **multi-select** all of the outfit shapes in the list and choose **Copy Bone Weights** after a right-click.

    [![Copy Bone Weights](http://i.imgur.com/xlVgiZhm.png)](http://i.imgur.com/xlVgiZh.png)

9. Open up the **File -> Save Project As...** dialog and fill out all of the text fields. Make sure to carefully read all of the tooltips that appear when hovering over them, as they will tell you what to do.

    See the [[saving a project]] page for more details!

10. Save the project and you will immediately be able to select it, build it and apply your presets to it in the BodySlide part of the program.

11. (optional but recommended) Set up **groups** for your new outfit, so that presets for the specific body group become available for selection. A second, separate group can be used to provide an easy way to choose your projects for a batch build.

    To add an outfit to one or more groups, use the group manager accessible at the top-right of the BodySlide frame. You can save multiple groups into one XML file inside of the SliderGroups folder.

    See the [[group manager|Using the group manager]] page for more information on how to use it!

   _Note that if you add an outfit to its own group, do not forget to add it to the master group (for example "CBBE") as well!_

12. Share your projects! See the start of this page for info on how to do that.