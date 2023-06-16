#Thinkmax development best practices:
##Tables

####Considerations
<ul>
    <li></li>
</ul>

####Naming conventions
<ul>
    <li><b>Tables</b></li>
    <ul>
        <li>[Client prefix][description of purpose]</li>
        <ul><li>i.e. TMXSpecialOrderHeaderTable or TMXSpecialOrderLine</li></ul>
        <li>Description of purpose</li>
            <ul>
                <li>This part of the table name is significant and should adequately describe the data inside the table. The FDD or development hand-off between the developer and dev lead should name tables.
                </li>               
            </ul>
        <li>Temporary tables should end in "Tmp"</li>
    </ul>
    <li>Fields</li>
    <li>Indexes</li>
        <ul>
            <li>All table indexes end in "Idx"</li>
            <li>For the primary key of the table: [tableName]"Idx"</li>
            <ul><li>i.e. TMXSpecialOrderHeaderTableIdx</li></ul>
        </ul>
</ul>

####Required object properties
|Type|Required property|Value|
|-|-|-|
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
|Field|ExtendedDataType||
|Field|Mandatory<br><i>(If used as primary key field)|<b>Yes|
|Field|AllowEdit<br><i>(If used as primary key field)||
|Field group|Label||
|Relation|Cardinality||
|Relation|Related Table Cardinality||
|Relation|Related Table||
|Relation|Relationship Type|<b>Association|

Link to <a href="">Microsoft documentation</a>