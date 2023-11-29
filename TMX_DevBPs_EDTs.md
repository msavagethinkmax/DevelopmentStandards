##Extended data types 

####Considerations

* One custom extended data type per table field is <b>NOT</b> required in Thinkmax development. This had historically been the practice in TEC.
* The creation of an EDT should answer the following questions
  * Is there no relevant Microsoft object that can be re-used?
  * Does this extended data type need to be re-used?
  * Does this extended data type need to define something new in the system?
* The developer should opt to re-use or extend Microsoft EDTs where applicable, unless the development requires something completely custom to achieve the requirement.  
  * For example, if you are implementing a vehicle manufacturing solution and there is no good EDT that reflects a VIN number being stored, this scenario would require a new, custom EDT.
  * Another example could be if you need to control string size or a similar EDT property that cannot be accomplished through extensions.

####Required object properties
* Name (following best practice naming conventions)
* Label

#####Type specific properties

|Type|Required Property|Naming convention|
|:-|:-|:-|
||Name||
||Label||
|String|String size||
|Real|||
|Integer|||
|Date||Object name ends in "Date"|
|DateTime||Object name ends in "DateTime"|
|GUID||Object name ends in "GUID"|
|Container|||
|Enum|Enum type||

---
Link to [Microsoft documentation](https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/dev-ref/xpp-data-edt)


