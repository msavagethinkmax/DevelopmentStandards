##Data entities

####Considerations
* All new tables developed should have a corresponding data entity created, unless otherwise specified in the FDD or initiative. The development of a data entity should be assumed when estimating the creation of table(s).
* Make new data entities both data management enabled for access from the F&O UI and also Public, so that they are accessible through OData, unless otherwise specified.
####Naming conventions
* All data entity object names should end in "Entity".
* If the entity is exposed to OData via the IsPublic property.
  * Public collection name should be the plural form of the object name minus "entity".
  * Public entity name should be the singular form of the object name minus "entity".
  * For example an entity named TMXSpecialOrderLineEntity would have a public collection name of "TMXSpecialOrderLines" and a public entity name of "TMXSpecialOrderLine".
* There must be one EntityKey populated with the field(s) that make the entity record unique.

####Required object properties
|Type|Required property|Default value|
|:-|:-|:-|
|Data entity|Label||
||Primary Key|**EntityKey**|
||Data Management Staging If Data Management Enabled is set to Yes</i>||
||Public Collection Name <br>*If Is Public is set to Yes*||
||Public Entity Name <br>*If Is Public is set to Yes*||
|Data entity relation|Cardinality||
||Related Table Cardinality||
||Related Table||
||Relationship Type|**Association**|

---
Link to [Microsoft documentation](https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities)