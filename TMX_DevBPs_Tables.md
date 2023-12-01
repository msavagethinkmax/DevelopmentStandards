##Tables

####Considerations
 * The name of a table is significant and should adequately describe the data inside the table. The FDD or development hand-off between the developer and dev lead should name tables. Name should be meaningful but as concise as possible.
* Similarly, the name of a field is important because it lets anyone viewing or using the table what the purpose of the field is for, so that the correct data is assigned to the field. Names should be descriptive but also concise.            

####Naming conventions
* Tables
  * [Client prefix][description of purpose]
    * i.e. TMXSpecialOrderHeaderTable or TMXSpecialOrderLine
  * Temporary tables should end in "Tmp"
* Fields
  * Fields added to a table via extension should use the project or initiative prefix.
* Indexes
  * All table indexes end in "Idx"
  * For the primary key of the table: [tableName]"Idx"
  * i.e. TMXSpecialOrderHeaderTableIdx

####Required object properties
|Type|Required property|Default value|
|:-|:-|:-|
|Table|Label ||
||CreateRecIdIndex|<b>Yes|
||CreatedBy|<b>Yes|
||CreatedDateTime|<b>Yes|
||ModifiedBy|<b>Yes|
||ModifiedDateTime|<b>Yes|
||PrimaryIndex|<b>Yes|
||ReplacementKey <br><i>(if related to other tables via RecId)|<b>Yes|
||TitleField1||
||TitleField2||
||DeveloperDocumentation||
|Field|Label <br><i>(If overriding EDT label)||
||ExtendedDataType||
||Mandatory<br><i>(If used as primary key field)|<b>Yes|
||AllowEdit<br><i>(If used as primary key field)||
|Field group|Label||
|Relation|Cardinality||
|Relation|Related Table Cardinality||
|Relation|Related Table||
|Relation|Relationship Type|<b>Association|
