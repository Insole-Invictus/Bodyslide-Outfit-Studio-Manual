## Introduction
Projects for BodySlide are created and saved in the Outfit Studio part of the program. Their files store the information about the meshes and sliders that are used to make up the project.

Once you've created a conversion or project in Outfit Studio, for example after following one of the guides, you can use the **File -> Save Project As** menu item and the following dialog will appear.

![Save Project As](http://i.imgur.com/OXkWcBT.png)

## Filling out the fields
#### Display Name
The **name of the project**, as it will appear in the outfit list in BodySlide. This can be anything you want, but try to keep it relevant to the content.

#### To Project
This button **copies the current display name to the other project text fields** below. Unless you're creating a big pack of projects that requires custom folder structures, this button may be helpful to you.

#### Output File Name
The name of the output file of the project that **will end up in the game data path** after a build in BodySlide. **For Skyrim** (low/high weight output), this should **not** include _0 or _1 in the name. The file extension is not required, as it will automatically be appended when building.

#### Output Data Path
The location in the game's data path **where the output files will be placed** when building in BodySlide. This does **not** include the output file name (see image above).

#### Weight Output
This selection decides if the project will show a separate **low and high weight section** in the BodySlide UI and if the output files have **_0 and _1** appended to their file names, or not. Low/High weight output is currently used **for Skyrim only**.

#### Slider Set File
The name of the **project .osp file** that will be saved to the **SliderSets** folder. There can be **multiple projects** inside of one .osp file, so if you make a pack of multiple projects, you can reuse the same file.

#### Shape Data Folder
The folder inside of the **ShapeData** directory, where the **mesh and slider data** files will be saved to. This can include multiple subfolders, such as **Dress\Torso** or **Dress\Necklace**.

#### Shape Data File
The file name for the **meshes of the project** that will be saved to the shape data folder from above.

#### Copy reference shape into output
While you're working on a project in Outfit Studio, it's possible that you have a **reference shape** loaded, highlighted in green. This toggle decides if said reference shape should be **saved permanently into the project** for BodySlide, or if it should be ignored.