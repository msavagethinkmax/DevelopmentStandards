##Views

####Considerations
* Treat development of views similarly to table development, as a view is just a data structure flattened into a single data source.
* While not required, it is highly recommended to use AOT query objects to drive the view data sources to make maintenance of a solutions easier.

####Naming conventions
* View object names should end in "View".
* View object names should adequately describe the data that the view has been developed to represent, following similar considerations as naming tables.

####Required object properties
|Type|Required property|Default value|
|:-|:-|:-|
|View|Label ||
||TitleField1||
||TitleField2||
||Developer Documentation||