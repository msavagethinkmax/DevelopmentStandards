#Thinkmax development best practices:
##Label files

####Considerations
<ul>
    <li>Labels are convenient ways of standardizing and reusing static text in the system across translations. They avoid hard-coding text and provide a central point to implement static text used in the system.</li>
    <li>Before creating a custom label file, check to see if a label file for the same text exists in Microsoft's various label files and use that for your development.</li>
    <li>Label language localizations should be decided per project.</li>
    <li>There should be at least one label file per model.</li>
        <ul>
            <li>The project development lead is the main person responsbile for deciding label implementation.</li>
            <li>It is strongly recommended to implement a label file per FDD to reduce the usual merging complexity with multiple developers changing the same label file</li>
        </ul>
</ul>

####Naming conventions
<ul>
    <li>Each label ID should represent and summarize the label text for readability</li>
        <ul>
            <li>Label text "This is my custom label" would have ID "@CustomLabelFile:ThisIsMyCustomLabel" or "@CustomLabelFile:MyCustomLabel"</li>
            <li>From previous versions of Dynamics AX, most Microsoft label files are incremented numerically with their layer prefix like "@SYS12345". <br>Do <b>not</b> reuse this approach in custom development.</li>
        </ul>
</ul>

Link to <a href="">Microsoft documentation</a>