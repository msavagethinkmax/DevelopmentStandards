##Queries

####Considerations
* Queries are a reusuable AOT resource for accesssing a subset of data based on pre-defined criteria.  When writing query objects in X++, consider if the query needs to be re-used in the implementation and opt for an AOT query object instead.
* At least one data source is required per query object.

####Naming conventions
* All query objects created must end in "Query"

####Required object properties
|Type|Required property|Default value|
|:-|-|-|
|Query data source|Table||
|Query nested data source|Table||
||Relation||