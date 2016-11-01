## What are bone weights?
Bone weights are used for games that have **skeletal animation** systems. They tell the engine what parts of the mesh (which vertices) have to move along with one or more specific bones and how strong they are affected by the bone's movement (the weight factor).

This guide explains how to copy the bone weights from a reference, such as a body mesh, to other meshes like outfits. That way, everything will animate correctly in-game and the weighting matches up with the body.

It should work for any mesh or reference template that has the weights you need to copy inside of it. You need an otherwise 100% working outfit or mesh for this tutorial first, though!

## Step-by-step example
1. ![New Project](http://i.imgur.com/KxNNU2K.png) Create a **new project** in Outfit Studio.

2. Choose the NIF file or reference template that **has the weights you need** as a reference and click next.

3. Select the **outfit or mesh** you want to copy the weights of the reference to and click finish.

4. Multi-select all of the shapes you want to **copy the bone weights to** in the list to the right, then switch to the **bones tab** and select all bones to use with the CTRL key to multi-select. From here, use the **Shape -> Copy Selected Weights** menu item.

    ![Bones](http://i.imgur.com/hLNvRxL.png)

5. If you simply want to copy the weights **of all bones** and not choose them manually, use the **Shape -> Copy Bone Weights** menu item instead.

6. A weight copy settings dialog will pop up, where you can **customize the way the bone weights will be copied** from the reference to the selected shapes. Most of the time, the default settings are sufficient. Check the **[[weight copy options|Weight Copy Options]]** page for details.

7. Finally, use the **File -> Export -> Export NIF** menu item to save your changes. If what you were working on was a BodySlide project, then save that instead.