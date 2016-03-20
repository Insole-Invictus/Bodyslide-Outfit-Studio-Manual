## 3.3
- General: Changing settings now reloads archives properly.
- General: Changing the target game now recommends a default skeleton.
- General: The settings dialog can't be opened while Outfit Studio is active anymore.
- General: Stopped the texture pools of BS and OS conflicting with each other (black textures).
- General: Fixed crash when clicking both the left and right mouse button at the same time.
- General: Added Maya scripts for fixing the rig of FBX exports to the "res" folder.
- General: The 3D views now load/generate mipmaps to reduce texture artifacts.
- General: The 3D views can now load all texture compression formats (DXT1-5, BC1-7).
- General: Fixed Z-Buffer for the 3D views, which appeared as clipping, even though there was none.
- General: Fixed color profile warnings in the log.
- Outfit Studio: Added a transform tool (3D widget) to move/rotate shapes more easily.
- Outfit Studio: Holding down S key and scrolling while the transform tool is active will scale shapes.
- Outfit Studio: Added "Shape -> UV -> Invert X/Y" feature.
- Outfit Studio: Material file paths for FO4 can now be edited in the shape properties.
- Outfit Studio: Fixed FO4 crash that could happen for some zapped shapes.
- Outfit Studio: Added support for a few more block types (mostly for statics).
- Outfit Studio: Added "File -> Import -> Import NIF" feature.
- Outfit Studio: Added menu items to import/export BSClothExtraData blocks to HKX files.
- Outfit Studio: Added "Save Preset" feature to OS.
- Outfit Studio: Added "Remove Bone From Selected" feature to bone context menu.
- Outfit Studio: Fixed weighting not staying on a shape if it wasn't weighted to the bone before.
- Outfit Studio: Made bone context menu work without having to click on the name of a bone.
- Outfit Studio: Made it possible to add a custom bone to the project that's not in the ref skeleton.
- Outfit Studio: Fixed weighting colors only showing for the active shape, not all selected shapes.
- Outfit Studio: Fixed FBX import/export ignoring bones that aren't in the reference skeleton.
- Outfit Studio: Fixed crash for FBX import/export for shapes without normals or UVs.
- Outfit Studio: Double-clicking on a shape now opens its shape properties dialog.
- Outfit Studio: Stopped the RGB FaceGen shader flag from being a default for OBJ/FBX imports.
- Outfit Studio: Fixed "Save Project As" dialog not showing the loaded game data path for upper-case paths.
- Outfit Studio: Now saves the last size of the slider panel to the config file.
- Outfit Studio: Improved cursor/brush stroke performance.
- Outfit Studio: Fixed bone scaling preview for Skyrim.
- Outfit Studio: Fixed window parenting of some message boxes.

## 3.2
- General: Made the updating of mesh normals asynchronous for brush strokes and in the preview.
- General: Fixed crash when attempting to load certain material files.
- General: All text should now be readable with Windows font scaling or themes.
- BodySlide: Fixed preview not reloading properly if the NIF stayed the same but was zapped.
- Outfit Studio: You can now select and edit multiple shapes at the same time with brushes.
- Outfit Studio: Added a new toggle "Global Brush Collision" for toggling active/selected meshes collision.
- Outfit Studio: NiExtraData blocks can now be edited in the shape properties (NiStringExtraData for now).
- Outfit Studio: Fixed "Load Project" not setting the reference shape properly for non-external references.
- Outfit Studio: Loading old .xml projects now adjusts the slider set file name to .osp automatically.
- Outfit Studio: Fixed slider data imports for FO4 sometimes introducing noise due to lower precision.
- Outfit Studio: Fixed various issues/crashes with the faces section of the OBJ import.
- Outfit Studio: Fixed OBJ/FBX import and FBX export for FO3NV.
- Outfit Studio: Renamed/shortened a few menu items.

## 3.1c
- General: Fixed the loading of loose material files that aren't in BA2 archives.
- General: Added toggle for the batch build override dialog to the settings.
- BodySlide: Added additional mouse camera controls to the preview window.
- Outfit Studio: Exporting slider data to OBJ works as intended again now.
- Outfit Studio: Fixed OBJ import crash because of #comments in the faces section.
- Outfit Studio: Fixed OBJ import not loading triangles properly for some faces sections.
- Outfit Studio: Fixed BSSkinInstance target reference for OBJ/FBX import.

## 3.1b
- General: Now saves the last window state to the config file (maximized window or not).
- BodySlide: Batch building now notifies you of any overrides and asks you which one to build.
- BodySlide: Renamed "Save Preset" button to "Save Preset As...".
- BodySlide: Added new button "Save Preset" that transfers the changed slider values to the preset file.
- BodySlide: Fixed preset drop down selection after saving a new preset to file.
- BodySlide: Now immediately updates the normals when opening a new preview.
- BodySlide: Now immediately activates zaps from presets in the preview.
- Outfit Studio: Added new hotkeys for the view modes (Shift+1 to 5).
- Outfit Studio: Added two buttons to the tool bar: "X-Mirror and "Edit Connected Only".
- Outfit Studio: Fixed BSEffectShaderProperty export.
- Outfit Studio: Now allows multiple BSClothExtraData to be selected for export at once.
- Outfit Studio: Fixed crash when attempting to edit a slider after swapping between projects.
- Outfit Studio: Fixed slider edit mode not closing after swapping between projects.
- Outfit Studio: Fixed name copying for alpha properties.
- Outfit Studio: Fixed crash when copying weights while there are no bones loaded.

## 3.1a
- General: Fixed crash for a very specific type of .BSA archive (empty folder name).
- General: Added a warning that shows if there's no read/write permission for the game data path.
- General: Fixed log output for fatal and unhandled exceptions, properly lock the program thread.

## 3.1
- BodySlide: Slider categories are now sorted by order, not by alphabet.
- Outfit Studio: Fixed crash when saving a project without sliders or shapes loaded.
- Outfit Studio: Removed "Apply the shape changes?" dialog and always apply immediately.
- Outfit Studio: Fixed various bugs with adding bones to a project through the UI.
- Outfit Studio: Weights of bones not present in the ref. skeleton can now be viewed and edited.
- Outfit Studio: Fixed NiNode alignment for meshes will a full skeleton hierarchy (Skyrim HDT PE).
- Outfit Studio: Fixed FBX import/export for Skyrim as the target game.
- Outfit Studio: Fixed shader name and wet material reference copying.
- Outfit Studio: Fixed various .OBJ bugs.
  - Fixed loading OBJs that don't have an object name in them.
  - Fixed OBJs without UVs crashing FO4 shape creation.
  - "template/OutfitTemplate_Wet.bgsm" is the default wet shader now.
  - Don't link any default material .bgsm to the shader name yet.

## 3.0a
- General: Now looks for material files (BGSM/BGEM) and loads their diffuse textures.
- General: Fixed NIF corruption if the root children contained an empty reference.
- General: Fixed camera panning for a certain zoom level.
- BodySlide: Fixed zaps not being updated properly in the preview while it's open.
- Outfit Studio: Added selection for which BSClothExtraData to use on export/save.
- Outfit Studio: Updated BSEffectShaderProperty support.
- Outfit Studio: Fixed copying of NiAlphaProperty values.
- Outfit Studio: Fixed weight brush when a dialog box appeared while holding ALT.
- Outfit Studio: Removed progress dialog and added a progress bar instead.
- Outfit Studio: Now refreshes the outfit list in BodySlide automatically when saving a new project.
- Outfit Studio: Fixed absolute paths for Shape Data Folder in Save As dialog.
- Outfit Studio: Cleaned up the New Project, Load Reference and Load Outfit dialogs.

## 3.0
- General: Fallout 4 support!
- General: Support for loading textures from BA2 archives.
- General: Added 64-bit executable build.
- General: Added archive selection and more improvements to the settings dialog.
- General: New file formats .osp and .osd:
  - .osp files contain the slider sets/projects (XML format).
  - .osd files contain the slider data merged into one file (binary format).
- BodySlide: Sliders now have a separate display name stored in the category file(s).
- Outfit Studio: Added FBX import and export support (Autodesk FBX SDK).
- Outfit Studio: Added drag and drop support for NIF, FBX and OBJ files.
- Outfit Studio: Added drag and drop support for BSD and OBJ slider files.
  - Drop on a slider to update it or hold the CTRL key to create a new slider.

## 2.8d
- BodySlide: Fixed preview window update when using certain zaps.
- Outfit Studio: Fixed bug of v2.8c when loading the weighting.

## 2.8c
- General: Added logging functionality.
- General: Starting this version, the program is now licensed under the GPLv3+.
- BodySlide: Fixed layout bugs for single-weighted sets (slider frame and preview window).
- Outfit Studio: Merged reference shape and outfit shapes list into the same tree.
- Outfit Studio: The reference shape is highlighted with bold, green text now.
- Outfit Studio: Shapes can now be reordered in the list with a drag and drop.
- Outfit Studio: Exported NIF files now have their shapes in the same order as Outfit Studio.
- Outfit Studio: Added transparency settings to the shape properties dialog.
- Outfit Studio: Added menu item to set a new reference shape.

## 2.8b
- BodySlide: Fixed Group Manager using old groups or not saving in some cases.
- Outfit Studio: Added "Export Slider Data -> Export OBJ" feature (previously .BSD only).

## 2.8a
- BodySlide: Now shortly renders an empty preview when switching sets.
- Outfit Studio: Fixed TRI morphs import for unpacked TRI files (such as SAM).

## 2.8
- BodySlide: Merged preview windows and added a weight slider.
- BodySlide: Now updates preview window when switching sets, instead of closing it.
- BodySlide: Slightly reduced memory and video memory usage.
- Outfit Studio: Added a new properties dialog for shapes, currently for shader/texture editing (WIP).
  - Shader type, specular color/strength/power, emissive color/multiplier and texture paths.
- Outfit Studio: Fixed loading projects with externally referenced shape data.
- Outfit Studio: Fixed "Save Project As" sometimes removing textures and/or masks.
- Outfit Studio: Fixed zapping sometimes causing TRI morphs to not link to a shape properly.
- Outfit Studio: Fixed OBJ shape import applying wrong transform matrix.

## 2.7h
- General: Lots of under-the-hood code refactoring.
- Outfit Studio: Support for BSEffectShaderProperty and various shader animation controllers.

## 2.7g
- General: Fixed texture paths with backslash at the very front.
- Outfit Studio: Fixed outfit name not updating after the project has been saved under a new name.
- Outfit Studio: Added hotkey (F2) for renaming shapes. Changed deleting shapes from CTRL+Del to Del.

## 2.7f
- BodySlide: Batch building now uses the currently active slider values as well.
- BodySlide: Fixed copy slider values buttons affecting hidden sliders.
- BodySlide: The preview is now equally as bright as the Outfit Studio view.
- BodySlide: Fixed "Remove Group" in Group Manager being disabled by default.
- Outfit Studio: Added "Slider -> Export TRI Morphs" feature to Outfit Studio.

## 2.7e
- General: Minor performance improvements. 
- BodySlide: Fixed crashing preview windows caused by rendering at the wrong times. 
- BodySlide: Added buttons to copy slider values to either low or high weight. 
- Outfit Studio: Removed dialogs for virtual shape offset and scale (just the virtual ones). 
- Outfit Studio: Added a minus and plus button to slider edit mode that scales slider data (not the shape).

## 2.7d
- BodySlide: Fixed uncompressed files within BSAs not loading (textures in preview).
- BodySlide: Now rescans BSAs when Game Data Path was changed in the settings dialog.
- Outfit Studio: Fixed "Add Group" button of group manager being disabled by default.
- Outfit Studio: Fixed bones sometimes not or wrongly being erased from NiSkinData.

## 2.7c
- BodySlide: Added new settings dialog.
- Outfit Studio: Fixed weight brush bug introduced in 2.7.

## 2.7b
- Outfit Studio: Fixed conforming and weight copying bug introduced in 2.7. 
- Outfit Studio: "Load Slider Preset" function now shows all presets, no matter the set or group names. 
- Outfit Studio: Fixed weights and masks not being shown if no texture was found.

## 2.7
- BodySlide: Now scans BSA files for textures and loads them, if they weren't found as loose files.
- BodySlide: Added a group manager for editing and creating group files.
- BodySlide: Changed texture path trimming behavior again. Always only "textures" at the front.
- Outfit Studio: Added "Slider -> Import TRI Morphs..." feature.
- Outfit Studio: Integrated brush settings into the main frame.
- Outfit Studio: Disabled axis-crossing for conforming and weight copying.
- Outfit Studio: Improved weight brush performance.
- Outfit Studio: Changes to the way duplicate shapes are renamed.
- Outfit Studio: Added working directory before the ShapeData path for loading projects with Mod Organizer.
- Outfit Studio: Reference not needed for saving a project anymore.
- Outfit Studio: Shader controllers are not dropped anymore.
- Outfit Studio: Fixed various bugs related to using "Keep other shapes" when loading an outfit.
- Outfit Studio: Normals for skin shaded shapes in the outfit list aren't generated anymore.
- Outfit Studio: Added all conversion references to the template list, as shape names can now be defined.
- Outfit Studio: Fixed crash when hovering mouse over mesh too early.
- Outfit Studio: OBJ import correctly flips UVs again now.
- Outfit Studio: Fixed OBJ export for NiTriStripsData.
- Outfit Studio: Fixed minor issues with shape selection tree.

## 2.6
- BodySlide: Added "About" dialog with library info and licences.
- Outfit Studio: Move, scale and rotate shape dialogs now use sliders.
- Outfit Studio: Added preview to "Rotate Shape" dialog.
- Outfit Studio: Weight brush now has X-Mirror disabled by default.
- Outfit Studio: Added "Front/Back/Left/Right" view buttons that adjust the camera.
- Outfit Studio: Added perspective/orthographic projection toggle.
- Outfit Studio: Added field of view slider.
- Outfit Studio: Added more accurate zooming by holding the middle mouse button and shift key.
- Outfit Studio: Added light settings tab. The same settings are applied in the BodySlide previews.
- Outfit Studio: Added "Fixed Weight Brush" check box when in the bones tab.
- Outfit Studio: Added support for FO3/NV NIFs. You can't convert them between games, though!
- Outfit Studio: Added "Target Game" entry to the Config.xml.
- Outfit Studio: Refactored the NIF code, possibly including some fixes.
- Outfit Studio: Removed registry warning if the game data path has been manually set already.
- Outfit Studio: Renamed "Copy Name" button to "To Project" in the save project dialog.
  - Does not affect the "Output File Name" and "Output Data Path" text controls anymore.
  - Label now says "_0/_1.nif" or ".nif" depending on low/high or single-weighted outputs.
- Outfit Studio: Bone weighting preview is now cleared before saving/exporting.
- Outfit Studio: Updated progress bar texts.
- Outfit Studio: Added error for unsupported NIF file versions.
- Outfit Studio: Now using the TinyXML-2 library (previously 1)

## 2.5
- CBBE: Fixed "BigTorso" slider causing a wrist seam.
- Unified UNP: Adjusted belly weighting for UUNP HDT and UUNP Special.
- Outfit Studio: Added multi-select functionality to shape list (e.g. "Move Shape" for all selected ones).
- Outfit Studio: Added "File -> Apply Overall Skin Transform". Disable to try out different offset loading.
- Outfit Studio: Added "File -> Export -> Export NIF With Reference". Exports full project, instead of just outfit.
- Outfit Studio: Fixed "Save Project" keeping deleted bone nodes of reference shape.
- Outfit Studio: Fixed "SliderSets" folder not being created if non-existent.
- Outfit Studio: Fixed crash on out-of-range zap index from old slider data.
- Redone OpenGL canvas with wxGLCanvas from wxWidgets.

## 2.4
- CBBE: Fixed "CBBE Vanilla" and "CBBE Vanilla NeverNude" mesh seams.
- Unified UNP: Improved, cleaned and unified the weighting of the 4 body types.
- Outfit Studio: Fixed Save Project always clearing the mask, even though there were no unweighted vertices.
- Outfit Studio: Load Project now loads shapes with slider data that is in a different folder, instead of removing them.
- Outfit Studio: Fixed "Show Mask" toggle affecting the visibility of the bone weights as well.
- Outfit Studio: Added "Transfer Selected Weights" menu item:
  - Transfers the weights of the selected bones from reference to chosen shape 1:1.
  - Requires same vertex count and order of source and target shape.
- Outfit Studio: Added "Apply Sliders?" message to the "Load Slider Preset" dialog as well.
- Outfit Studio: Added a brush that smooths bone weighting, accessed by pressing the SHIFT key while weight painting.
- Outfit Studio: Added NiTriStrips support (apart from "Build Skin Partitions").
- Outfit Studio: Added NiSkinPartition support.
- Outfit Studio: Added a bone scaling preview slider to the bones tab.

## 2.3
- BodySlide: Added "RaceMenu Morphs" build feature for in-game sliders. Requires RaceMenu and a matching morphs plugin.
- Outfit Studio: Added tons of conversion references for CBBE -> X -> CBBE (in UNPConvert.xml) and restructured them.
- Outfit Studio: Updated the XPMS Extended reference skeleton to version 2.50.
- Outfit Studio: Edited the reference skeleton to hopefully fix hand/finger scales when exported.
- Outfit Studio: Fixed crash when renaming shapes with unusual slider data naming, usually very old or manually edited.
- Outfit Studio: Added value display showing the mask factor of the current vertex while the mask brush is active.
- Outfit Studio: Added value display showing the position of the current vertex while any transform brush is active.
- Outfit Studio: Added single vertex movement dialog that shows when the 'V' key is pressed.
- Outfit Studio: Merged "Missing Bone" messages on a per-shape basis and added a few new error messages.
- Outfit Studio: Added ability to close the Move/Rotate/Scale Shape and brush settings dialogs with the enter key.
- Outfit Studio: Fixed "Duplicate Shape" and "Coalesce sliders" dialogs not being cancelable.
- Outfit Studio: Adjusted default brush settings and reorganized the brush settings dialog.
- Outfit Studio: Implemented automatic trimming of "Data\textures\" in texture set paths of shapes (for BS too).
- Outfit Studio: Added new button "Apply Diffuse" for the "Set Textures" dialog to apply texture changes to the view.
- Outfit Studio: Implemented automatic appending of file extensions in the "Save Project As" dialog (not visible).
- Outfit Studio: Fixed moving shapes in slider edit mode to work as intended.
- Outfit Studio: Added "Copy Selected Weights" to the shape context menu as well.
- Outfit Studio: Fixed resizing the brush with the 'S' key going over the limits.
- Outfit Studio: Changed hotkeys for brush size/strength adjustments to: Shift + +, Shift + -, Ctrl + +, Ctrl + -
- Outfit Studio: Bones that are not in the reference skeleton will not be removed when a weight copy is done anymore.
- Outfit Studio: The duplicate reference shape in the outfit shape list is now automatically deleted when loading a project.
- Outfit Studio: Loading projects with only one slider set in the XML file skips the selection dialog now.
- Outfit Studio: Made the load and save project file picker dialogs default to the "BodySlide\SliderSets" folder.
- Outfit Studio: Increased slider knob size (OS).

## 2.2d
- Outfit Studio: updated the XPMS Extended reference skeleton to version 2.33. 
- Outfit Studio: fixed "Brush -> Clear Mask" clearing weight colors as well (instead of only the mask). 
- Outfit Studio: weights are now only copied to unmasked vertices. Masked vertices keep their old weights. 
- BodySlide: fixed category UI alignment of single-weighted slider sets. 
- Now requires "Microsoft Visual C++ 2013 Redistributable (x86)" instead of 2012. Get it from Microsoft if it's not installed. 
- No longer Windows XP compatible (BodySlideWXP.exe removed).

## 2.2c
- BodySlide: fixed activating a zap after a preview window has been opened once causing a crash
- BodySlide: fixed what's getting batch built sometimes not representing the selection in the dialog
- BodySlide: widened the body/outfit drop down list by a bit
- Outfit Studio: fixed absolute path issues in the Save Project As dialog and cleaned it up some
- Outfit Studio: fixed weight painting colors sometimes not getting removed from rendering
- Outfit Studio: making or loading a new project now clears all memory of the previous project
- Outfit Studio: added some message boxes telling you to select a shape before doing stuff first

## 2.2b
- Outfit Studio: fixed brushes not always rendering properly
- BodySlide: fixed crashes with certain slider sets (e.g. CBBE Feet)

## 2.2a
- BodySlide: fixed low preview not updating properly

## 2.2
- added basic texture alpha rendering for meshes
- fixed OpenGL panel of Outfit Studio getting focused even though the BodySlide frame is active
- fixed trying to render meshes without at least one triangle
- BodySlide: added slider categories UI for CBBE, customizable under "BodySlide\SliderCategories"
- BodySlide: fixed shapes without at least one triangle not getting deleted on build
- Outfit Studio: fixed crash when using "Copy Selected Weights" while a reference shape is selected
- Outfit Studio: fixed unweight and unmask brushes not using the strength settings of the weight/mask brushes
- Outfit Studio: updated the XPMS Extended reference skeleton to version 2.14 (same as 2.13)

## 2.1c
- Outfit Studio: updated the XPMS Extended reference skeleton to version 2.13

## 2.1b
- Outfit Studio: updated the XPMS Extended reference skeleton to version 2.11
- Outfit Studio: black spots issue - implemented fix for more precise tangent spaces calculation

## 2.1a
- reverted "Smooth Seam Normals" selection back to the way it worked in 2.0.0.10
- removed auto-fill from "Save Project As" dialog, but improved default value filling
- fixed that you could save projects without a valid reference shape loaded
- renamed default names and UI items for making new zaps (removed the "slider" because it's not a slider in BS)

## 2.1
- added and made the XPMS Extended (XPMSE) skeleton the default reference
- fixed bones from previous outfit carrying over to the others
- added numeric value display to OS, showing the weight factor of the current vertex to the current bone
- added a warning about unweighted vertices to the export/save that puts those under a mask automatically
- fixed a crash when loading a reference shape that didn't have a BSLightingShaderProperty
- it is now possible to create new sliders with spaces in their names in Outfit Studio
- fixed crash when using "Move Shape" in an empty project
- fixed some internal name assignments for slider sets and groups in BodySlide
- fixed slider sets not assigned to any group being hidden in the BodySlide outfit list
- changed unused check box in OS into a check/uncheck all sliders feature (for conforming)
- added slider range setting to Config.xml for BodySlide UI (SliderMinimum and SliderMaximum)
- fixed empty reference shape when loading a project that only had one shape in it
- fixed some focus problems with the BodySlide frame and scrolling slider view
- slider names in BodySlide now scale dynamically and are centered
- added non-virtual "Scale Shape" feature (actually modifies the vertices)
- added "Clean" and "Batch Clean" features that remove target files and can be used by holding down the ALT key
- fixed not being able to delete some shapes that didn't have a (normal) shader
- fixed various issues with special characters in file names
- fixed crash for templates that don't have a shape called "BaseShape"
- fixed crash for zap sliders in single-weighted slider sets (GenWeights=false)
- disabled "Smooth Seam Normals" by default for all outfit shapes (enabled for bodies)
- fixed some incorrect values when saving presets
- fixed opening slider properties causing loss of slider data
- fixed math of Outfit Studio frame position values stored in Config.xml
- fixed brush settings getting outside of their minimum and maximum values
- fixed weight brush being selectable outside of weight edit mode
- renamed move/offset/scale features for less confusing names (non-virtual and virtual edits)
- added live preview for Move Shape and Scale Shape dialogs (non-virtual and virtual)
- fixed weighting colors/masks not showing up and darkened textures for some GPU (shader syntax error)
- fixed "Do you want to apply your changes?" dialog causing other shapes to be reset
- added "Rotate Shape" feature to Outfit Studio
- added check box "Keep other shapes" to "Load Outfit" dialog, making mashups possible
- added "select all" and "select none" to the batch build dialog
- added double-sided rendering when enabled in shader (brushes not working with it yet)
- made it possible to remove masks by holding the ALT key and add masks in weight edit mode
- weight painting now honors the current mask, and so does copying bone weights
- fixed one of the issues causing black spots for shapes with two faces in an opposite direction
- changed OS mouse controls: LMB = paint, MMB/Shift+RMB = pan, RMB = rotate
- added Config.xml option to enable LMB panning mouse controls again for OS
- fixed duplicating a shape resetting changes (vertices, weights, texture settings)
- integrated conversion references and fixes that were previously uploaded separately (7B, CHSBHC, ADEC, CBPE)
- added "Group Aliases" to the Config.xml, allowing a merge of several preset groups into one for compatibility
- made CB++ presets compatible with CBAdvanced outfits and the other way around using group aliases
- made "Save Project" become available after a slider set was loaded
- fixed "Save Project" breaking slider set files (.nif file name)
- changed default values of sliders made using "New Zap Slider" to 100% for low and high
- fixed crash when importing .obj files without UV's into OS (UV's are important)
- fixed "Save Project" dialog not getting filled with current project information
- fixed crash when saving shapes that don't have BSDismemberSkinInstance nodes

## 2.0.0.10
- fixed a crash when setting base shape with outfit tree header selected
- added new exe BodySlideWXP.exe to test compatability with Windows XP (worked)
- corrected an issue with saving low-weight presets
- fixed an issue where adding a new slider to a reference loaded from a NIF wouldn't correctly use the morph data
- fixed a corruption in an output NIF when a skin shaded shape also had normals
- set BodySlide.exe to require admin rights on launch

## 2.0.0.9c
- minor package change, put BodySlide folder inside Data/CalienteTools for NMM compatibility

## 2.0.0.9b
- Beta version! Releasing to the public! Warning: may never get out of beta, and there are likely major problems, use at your own risk! :)
- fixed an issue that caused batchbuild to ignore the disabled outfits when building
- fixed an Outfit Studio problem that occurred when an outfit NIF had multiple shapes with the same name. Duplicated named shapes are now renamed to something unique.
- combined CalienteBody with CB++, it's now called CalienteBodyAdvanced, with 50+ sliders!