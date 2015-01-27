## 2.2d
- CBBE Body HDT: fixed symmetry of bone "Breast L R". 
- CBBE Body HDT: removed bone "Breast01 L R" as it's unnecessary for HDT PE. For animations use "CBBE Body TBBP". 
- CBBE Body HDT: smoother transitions for bones "Clavicle L R" and "Butt L R". 
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
- fixed offset of "CBBE Body TBBP"
- removed auto-fill from "Save Project As" dialog, but improved default value filling
- fixed that you could save projects without a valid reference shape loaded
- renamed default names and UI items for making new zaps (removed the "slider" because it's not a slider in BS)

## 2.1
- added and made the XPMS Extended (XPMSE) skeleton the default reference
- renamed "CBBE Advanced" to "CBBE Body", the main group is still called "CBAdvanced" for compatibility reasons
- added new "CBBE Body HDT" by ChronoTrigger77 to BodySlide (breast, butt and belly weights, previously "CT77 Body")
- added new "CBBE Feet" set by ChronoTrigger77 to BodySlide
- added new "NippleAreola" slider to all CBBE body sets
- improved slider quality for included undies sets (done by ChronoTrigger77)
- minor fixes and weight adjustments for all included meshes (done by ChronoTrigger77)
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