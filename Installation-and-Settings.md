## Installation
Simply download the program from one of its mod pages and extract it to your game's data folder.

Making use of mod managers is recommended, as well as keeping the program in the default folder provided with the download for the specific game, as this will make installing addons easier.

Before trying to configure the program, make sure you have set up a proper installation.

* When using mod managers, please follow the instructions provided on the mod pages for running BodySlide.
* Generally, make sure to read the description of the mod page you downloaded BodySlide from.

## Target Game
When running the executable for the first time, the following dialog window will show.

[![Target Game](http://i.imgur.com/i1K4gn0m.png)](http://i.imgur.com/i1K4gn0.png)

Select the "Data" folder of the game you want to use both BodySlide and Outfit Studio for and continue.

Games that are found in the registry will automatically have their paths filled out, but you can only choose one target game at the same time. You can change this selection later on in the settings dialog.

## Settings
The settings dialog of the program can be accessed from the main BodySlide window.

[![Settings](http://i.imgur.com/XgFCuDlm.png)](http://i.imgur.com/XgFCuDl.png)

### Game
**Target Game**  
The game you intend to use both BodySlide and Outfit Studio for. Changing this option will adjust the game data path and reference skeleton as well, make sure they're correct.

**Game Data Path**  
This path is supposed to point to the "Data" folder of the active target game. It is used for telling the program where to load resources from and build the output files of projects to.

### General
**Override Warning**  
Enables or disables the selection dialog that appears when multiple projects in a batch build are overriding the same output files.

**Left Mouse Pan**  
Enables or disables panning with the left mouse button in Outfit Studio. Bear in mind that the left mouse button is also used for brush actions.

**BSA Textures**  
Enables or disables scanning BSA/BA2 archives in the data folder for resources, such as textures for the preview windows.

**Use System Language**  
This enables the translation of BodySlide for the current system language of the computer, as long as the translation files exist.

### Data Files
A selection of all BSA/BA2 archives that are scanned for resources as needed, such as material or texture files. Try to keep these to a minimum for performance reasons.

### Reference Skeleton
**File**  
This is the reference skeleton file that Outfit Studio uses to create a list of bones and read bone transforms from.

**Root Node**  
The root node name can differ from game to game. It needs to be correctly set up in order for Outfit Studio to know where to start reading the list of bones from.

## Config.xml
A few options are currently only found in the Config.xml file directly.

**GroupAliases**  
Group aliases provide a way for presets saved under older group names to still apply when a group has been renamed. You can also merge several groups into one by linking them to eachother.

**SliderMinimum and SliderMaximum**  
Sets the minimum and maximum slider values for the BodySlide UI. This allows you to experiment more easily with sliders. There might be clipping outside of the 0-100 range and it's not supported!