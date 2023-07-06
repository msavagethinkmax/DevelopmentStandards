##Data entities

####Considerations
<ul>
    <li>All new tables developed should have a corresponding data entity created, unless otherwise specified in the FDD or initiative. The development of a data entity should be assumed when estimating creating table(s).</li>
    <li>Make new data entities both data mangement enabled for access from the F&O UI and also Public, so that they are accessible through OData, unless otherwise specified.</li>
</ul>

####Naming conventions
<ul>
    <li>All data entity object names should end in "Entity"</li>
    <li>If the entity is exposed to OData via the IsPublic property</li>
    <ul>
        <li>Public collecion name should be the plural form of the object name minus "entity"</li>
        <li>Public entity name should be the singular form of the object name minus "entity"</li>
        <li>For example an entity named TMXSpecialOrderLineEntity would have a public collection name of "TMXSpecialOrderLines" and a public entity name of "TMXSpecialOrderLine"</li>
    </ul>
    <li>There must be one EntityKey populated with the field(s) that make the entity record unique.</li>
</ul>

####Required object properties
|Type|Required property|Value|
|-|-|-|
|Data entity|Label||
||Primary Key|<b>EntityKey</b>|
||Data Management Staging <br><i>If Data Management Enabled is set to Yes</i>||
||Public Collection Name <br><i>If Is Public is set to Yes</i>||
||Public Entity Name <br><i>If Is Public is set to Yes</i>||
|Data entity relation|Cardinality||
||Related Table Cardinality||
||Related Table||
||Relationship Type|<b>Association</b>|

<hr>
Link to <a href="https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities">Microsoft documentation</a>