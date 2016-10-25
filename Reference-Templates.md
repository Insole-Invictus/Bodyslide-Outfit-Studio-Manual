## What are reference templates?
Reference templates are defined in the [RefTemplates.xml](../blob/dev/RefTemplates.xml) file and will appear in the **Load Reference** dialog.

![Template](http://i.imgur.com/RirpEsF.png)

They are shortcuts to loading specific shapes of existing projects into Outfit Studio as a [[conversion reference|Conversion references and using them]]. However, don't confuse these to be the actual project files - they are merely linking to them.

## Defining your own templates
To add your own template to the XML file, use the following syntax.
```xml
<RefTemplates>
    <Template sourcefile="SliderSets\CBBE.osp" set="CBBE Body" shape="CBBE">CBBE Body</Template>
    <Template>...</Template>
    <Template>...</Template>
</RefTemplates>
```

* The **sourcefile** attribute describes the path to the file your project is stored in. It is relative to the working directory (the BodySlide folder).
* The **set** attribute contains the name of the project inside of the .osp file to load as the reference.
* The **shape** attribute is the name of the mesh that will be become the reference shape. Only one shape can be the reference at the same time. You can find all shape names of the project in the .osp or .nif files
* To give the reference template your own name as it will appear in the list, adjust the text inside of the **Template** element.

If you want a project to appear as a template in Outfit Studio, but be invisible to end users in BodySlide, you can keep the .osp file outside of the **SliderSets** directory, such as the **ConversionSets** folder.