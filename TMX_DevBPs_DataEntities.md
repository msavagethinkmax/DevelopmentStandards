#Thinkmax development best practices:
##Data entities

####Considerations
<ul>
    <li></li>
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
</ul>

####Required object properties
|Type|Required property|Value|
|-|-|-|
|Data entity|Label||

Link to <a href="https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities">Microsoft documentation</a>