Most of the BodySlide and Outfit Studio user interface can be translated into any other language. This is done through funtionality built into the [wxWidgets](https://www.wxwidgets.org/) GUI library.

## Creating translations
To help out with **creating or editing translations**, you should get the free version of the program **[Poedit](https://poedit.net/)**. They can also be modified with any regular text editor and then compiled with Poedit, but that's not recommended.

[![Poedit](http://i.imgur.com/hz8LYKHt.png)](http://i.imgur.com/hz8LYKH.png)

Find the existing **BodySlide.po** file in the folder of the translation you want to edit.  
Examples:
* _BodySlide\lang\<language code>\BodySlide.po_
* _[BodySlide\lang\de\BodySlide.po](../blob/dev/lang/de/BodySlide.po)_

If the .po file is empty and you want to create a new translation, open up the [lang\BodySlide.pot](../blob/dev/lang/BodySlide.pot) template instead.

Now that you've opened up either a template or existing translation, you can start editing. To update a .po translation with new entries that have been added to the .pot template, choose **Catalogue -> Update from POT file** in Poedit.

![Update from template](http://i.imgur.com/C3c8o1L.png)

Make sure to provide both the **.po** (source text) and **.mo** (compiled text) of your translations in **[pull requests](../../pulls)**, so that everyone can benefit from them!

## Using translations
To actually change the language that's being used, open up the settings dialog and toggle the **Use System Language** check box (see [[Getting Started]]).

It is currently not possible to manually pick a specific language - this will be added at some point in the future.