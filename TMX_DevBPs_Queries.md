#Thinkmax development best practices:
##Queries

####Considerations
<ul>
    <li>Queries are a reusuable AOT resource for accesssing a subset of data based on pre-defined criteria.  When writing query objects in X++, consider if the query needs to be re-used in the implementation and opt for an AOT query object instead.</li>
    <li>At least one data source is required per query object</li>
</ul>

####Naming conventions
<ul>
    <li>All query objects created must end in "Query"</li>
</ul>

####Required object properties
|Type|Required property|Value|
|-|-|-|
|Query data source|Table||
|Query nested data source|Table||
||Relation||