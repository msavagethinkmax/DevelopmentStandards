##Extended data types 

####Considerations
<ul>
<li>One extended data type per table field is <b>NOT</b> required in Thinkmax development</li>
<li>The creation of an EDT should answer the following questions</li>
    <ul>
        <li>Is there no relevant Microsoft object that can be re-used?</li>
        <li>Does this extended data type need to be re-used?</li>
        <li>Does this extended data type need to define something new in the system?</li>
    </ul>
</ul>

####Required object properties
<ul>
    <li>Name (following best practice naming conventions)</li>
    <li>Label</li>
</ul>
#####Type specfic properties
|Type|Required Property|Naming convention|
|-|-|-|
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

<hr>
Link to <a href = "https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/dev-ref/xpp-data-edt">Microsoft documentation</a>


