Most of the BodySlide and Outfit Studio interface can be translated into any language. This is done using features  built into the wxWidgets framework the program is using.

To help out with **creating or editing translations**, you should get the free version of the program **[Poedit](https://poedit.net/)**. They can also be modified with any regular text editor and then compiled with Poedit, but that's not recommended.

Find the existing **BodySlide.po** file in the folder of the translation you want to edit.  
Examples:
* _BodySlide\lang\<language code>\BodySlide.po_
* _[BodySlide\lang\de\BodySlide.po](../blob/dev/lang/de/BodySlide.po)_

If the .po file is empty and you want to create a new translation, open up the [lang\BodySlide.pot](../blob/dev/lang/BodySlide.pot) template instead.

Now that you've opened up either a template or existing translation, you can start editing. To update a .po translation with new entries that have been added to the .pot template, choose **Catalog -> Update from POT file** in Poedit.

Make sure to provide both the **.po** (source text) and **.mo** (compiled text) of your translations in **[pull requests](../../pulls)**, so that everyone can benefit from them!