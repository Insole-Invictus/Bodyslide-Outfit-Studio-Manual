## Introduction
This guide will show you the steps required to update a project to a new version of the reference or body that was used, so that **new sliders will work** and become available in BodySlide.

The reference with its sliders has to be **swapped out** for the updated one without breaking the already existing slider data for the project.

## Step-by-step example
1. ![Load Project](http://i.imgur.com/viWOwuL.png) Load the project that you want to update using **File -> Load Project**.

2. Choose the updated reference in the **File -> Load Reference** dialog. This adds the new sliders and base mesh to the loaded project.

3. Any zaps or extra sliders the project had before are now gone, but **you can restore them** without having to recreate them from scratch (see optional steps below).

4. (optional) Use the **Slider -> New Slider** menu item to create any zaps or extra sliders the outfit had by typing the EXACT same slider name into the text field! The slider is now back and working the same way as before, you just need to set it to act as a zap again.

5. (optional) Now, enter the edit mode and **Slider -> Properties** (TAB) of each extra slider/zap you added back to the project and **make sure they are correct** (was it a zap, was it hidden, what are the correct default values).

6. Next, **uncheck all slider checkboxes** in the list to the right and then **select only those of the newly added or changed sliders**. That way, the previous slider data of the other sliders that weren't changed stays the same and you don't have to fix clipping for those again.

7. Use the **Slider -> Conform All** menu item. This conforms the all shapes in the project to the new sliders that are currently checked.

8. Finally, **[[save the project|Saving a project]]** and it should now make use of the updated reference and include the latest sliders.