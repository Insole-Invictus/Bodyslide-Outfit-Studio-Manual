## Introduction
Conversion references consist of one or more sliders that morph a mesh **from one shape to another**.

This guide outlines the steps needed to create your own conversion reference, so that you can convert outfits using it afterwards. There are **two ways** of accomplishing this.

## The convenient way
This method tries to **make use of existing sliders** in Outfit Studio to create a shape that resembles the conversion reference you want to create. This means you don't have to use 3D software such as Blender or 3ds Max.

1. **Load up a [[reference template|Reference Templates]]** that has enough sliders to make use of, for example the **CBBE Body** template.

2. Play around with the sliders to create a shape that looks **as close to your target as possible**. Don't forget that you can type in negative slider values or values above 100% as well.

3. When you're done, use the **File -> Make Conversion Reference** menu item and give the slider a name like "Your Target -> CBBE".

4. ![Edit Mode](http://i.imgur.com/qiGhRPw.png) Enter the edit mode of the newly created slider by clicking the pencil button beneath it, then export its shape using **Slider -> Export Slider Data -> Export OBJ**. You will need this OBJ file in a later step.

5. **Save the conversion reference project** (Target Body -> CBBE) using **[[File -> Save Project As|Saving a project]]**. For conversion references, the output paths and file names don't matter all that much, as they're only used to convert and are usually not used in BodySlide.

    The individual text boxes all have tool tips that appear when hovering over them with the mouse. You can **simply enter a display name** and click the **To Project** button.

6. ![New Project](http://i.imgur.com/KxNNU2K.png) Create a **new project** using the same reference template you used before, such as **CBBE Body**.

7. Add a new slider using the **Slider -> New Slider** menu item and name it "CBBE -> Your Target".

8. ![Edit Mode](http://i.imgur.com/qiGhRPw.png) Enter edit mode of the newly created slider by clicking the pencil button beneath it and use **Slider -> Import Slider Data -> Import OBJ** to load the shape you exported in step 4.

9. Keep the edit mode of the slider enabled and use **Slider -> Negate Slider**.

10. **Save the conversion reference project** (CBBE -> Target Body) using **[[File -> Save Project As|Saving a project]]**. For conversion references, the output paths and file names don't matter all that much, as they're only used to convert and are usually not used in BodySlide.

    The individual text boxes all have tool tips that appear when hovering over them with the mouse. You can **simply enter a display name** and click the **To Project** button.

11. You can now use the newly created conversion references together with Outfit Studio and morph outfits from body to body.

## The accurate way
For this, you will **need 3D software** such as Blender or 3ds Max. Unfortunately I can't explain how to use these programs here as it's out of scope, sorry. :wink:
 
In the following steps, the **target body** is the body you want to make conversion references for.

1. Load the **NIF file of the target body** into Outfit Studio and export its shape as an OBJ file using the **Shape -> Export Shape to OBJ** menu item.

2. Load the **CBBE Body** [[reference template|Reference Templates]] (or similar) into Outfit Studio and export its shape as an OBJ file using the "Shape -> Export Shape to OBJ" menu item.

3. **Import both of the just exported OBJ files** into your preferred 3D software. CBBE can used as a bridge to convert between various body types in our references, that's why it is used here as well.

4. Use **Shrinkwrap modifiers** or similar methods of your 3D software to wrap the CBBE shape around the target body (not the other way around!).

    Make sure to **manually align** the body shape a bit beforehand for better wrapping accuracy. You want all parts of the anatomy to line up properly before applying the wrapping. That way you get a CBBE body that looks somewhat like the target.

    #### Blender Shrinkwrap example
    ![Shrinkwarp](http://i.imgur.com/HvEksIQ.png)

5. Export the resulting shaped CBBE body (not the target body mesh) as an OBJ file. Make sure both the **vertex count and vertex order stay the same** by checking the export options of your program.

6. ![New Project](http://i.imgur.com/KxNNU2K.png) Create a **new project** in Outfit Studio using the same reference template you used in step 2.

7. Create a new slider using the **Slider -> New Slider** menu item.

8. ![Edit Mode](http://i.imgur.com/qiGhRPw.png) Click the edit button of the newly created slider and use the **Slider -> Import Slider Data -> Import OBJ** feature to create the "CBBE -> Target Body" slider data from the morph you exported out of the 3D software.

9. **Save the conversion reference project** (CBBE -> Target Body) using **[[File -> Save Project As|Saving a project]]**. For conversion references, the output paths and file names don't matter all that much, as they're only used to convert and are usually not used in BodySlide.

10. ![New Project](http://i.imgur.com/KxNNU2K.png) For a "Target Body -> CBBE" morph, create a **new project** once again and import the OBJ file of the **body that was wrapped around your target shape** (from above).

11. Add a new slider, click its edit button and load the morph from the OBJ file once again.

12. This time, invert the slider using the **Slider -> Negate Slider** menu item.

13. **Save the conversion reference project** (Target Body -> CBBE) using **[[File -> Save Project As|Saving a project]]**. For conversion references, the output paths and file names don't matter all that much, as they're only used to convert and are usually not used in BodySlide.

14. You can now use the newly created conversion references together with Outfit Studio and morph outfits from body to body.