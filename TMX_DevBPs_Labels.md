##Label files

####Considerations
* Labels are convenient ways of standardizing and reusing static text in the system across translations. They avoid hard-coding text and provide a central point to implement static text used in the system.
* Before creating a custom label file, check to see if a label file for the same text exists in Microsoft's various label files and use that for your development.
* Label language localizations should be decided per project.
* There should be at least one label file per model.
  * The project development lead is the main person responsbile for deciding label implementation.
  * It is strongly recommended to implement a label file per FDD to reduce the usual merging complexity with multiple developers changing the same label file.

####Naming conventions
* Each label ID should represent and summarize the label text for readability</li>
  * Label text "This is my custom label" would have ID "@CustomLabelFile:ThisIsMyCustomLabel" or "@CustomLabelFile:MyCustomLabel".
  * From previous versions of Dynamics AX, most Microsoft label files are incremented numerically with their layer prefix like "@SYS12345". <br>Do **not** reuse this approach in custom development.