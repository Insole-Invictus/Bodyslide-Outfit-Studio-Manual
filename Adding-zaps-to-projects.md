## What are zaps?
Zaps appear as sliders in Outfit Studio and as **check boxes** in BodySlide. They **remove previously defined parts** from meshes during a build of the project in BodySlide.

![Zaps](http://i.imgur.com/WOiBMue.png)

You can use them to add **optional parts** or accessories to your outfit projects for the user to toggle himself. Zaps can also be **hidden**, so that they can be used to remove parts of the body mesh to **prevent clipping**.

In Outfit Studio, they merely move the mesh around, but do not actually delete the parts.
Only BodySlide will remove the affected parts in the preview and builds.

## Step-by-step example
These steps show you how to create your own zaps. You need an otherwise already fully working project loaded for this and you need to make use of the mask brush.

1. ![Load Project](http://i.imgur.com/viWOwuL.png) Launch Outfit Studio and **load or create the project** you want to add zap options to.

2. ![Mask Brush](http://i.imgur.com/vktbaTu.png) Select the **mask brush** in the toolbar.

3. The area that you will be **masking** is the one that will **NOT be zapped away** (it will NOT be deleted and stays) when the zap is enabled in BodySlide.

4. If you want the opposite of what you masked to be zapped instead, choose the **Tool -> Invert Mask** menu item.

5. Use the **Slider -> New Zap Slider** menu item and **name the slider** appropriately. This creates the zap for what is **currently unmasked** for all selected shapes.

6. (optional) By going into edit mode of the zap and using any of the brushes on the mesh, you can **define more areas** that should be zapped later on, in case you missed any. Anything **affected by the slider** in Outfit Studio will be zapped later in BodySlide.

7. (optional) If you want a zap to be **always active and invisible** to the user of your project, activate the edit mode of the zap and enter the **Slider -> Properties** (TAB). In the dialog, set the **default value to 100** and enable the **hidden** checkbox.

    ![Zap Properties](http://i.imgur.com/NKkqtW1.png)

8. Finish the rest of your conversion if needed, then hit **[[File -> Save Project (As)|Saving a project]]** and follow on-screen tooltips. You can see and **test your new zaps** by selecting the project in BodySlide and opening the **preview window**.