##Classes

####Considerations
<ul>
    <li>Classes are created by developers to contain code in methods to perform a necessary function.</li>
    <li>Practice <b>encapsulation</b> when developing your classes and structures.  Classes should be created for a specific functionality.  Do not group multiple functionalities in the same class</li>
    <li>Be very mindful of the amount and reusability of your code.  If a functionality varies slightly from case to case, see if you can write a dynamic method to handle the variations, rather than writing multiple methods.<br>The same approach would apply to creating class structures. If you can create a base class to do the core function and create extension classes to handle the variations, this is preferable rather than having redundant objects and code.</li>
    <ul>
        <li>The consideration of this point is important to the code review process.</li>    
    </ul>
    <li>Extension classes
        <ul>
            <li>For project development, it is optimal to have one extension class per object per model.</li>
        </ul>
    </li>
    <li>Event handler classes
        <ul>
            <li>Follow Microsoft recommendation: opt for using a CoC method extension rather than an event handler.  Do not create an OnInserting table event handler method, extend the insert() method on a table.</li>
            <li>Do <b>not</b> mix event  handler methods across different objects in the same event handler class. All event handler methods in the event handler class should relate back to a single object.</li>
        </ul>
    </li>
</ul>

####Naming conventions
<ul>
    <li>Use camel-case in object naming</li>
    <li>Prefix <b>ALL</b> class names with the pre-defined project or initiative abbreviation (i.e. Thinkmax Vertical object names begin with "tmx").</li>
    <li>Make <b>meaningful</b> names for classes.</li>
    <ul>
        <li>The name of a class is important and should accurately detail the purpose of the class.</li>
        <li>If possible include the module and entity in the object name to define what area of the product it relates to (i.e. 'TMS', 'WHS', 'Sales', 'Invent', etc.)</li>
    </ul>
    <li>Extension classes
        <ul>
            <li>Table extension methods have "_T_" infixed. (i.e. tmxSalesTable_T_Extension)</li>
            <li>Form extension classes have "_F_" infixed. (i.e. tmxSalesTable_F_Extension)</li>
            <li>Form data sources have "_FDS_" infixed (i.e. tmxSalesTableSalesLine_FDS_Extension)</li>
            <li>Form data source data fields have "_DF_" infixed (i.e. tmxSalesTableSalesLineSalesPrice_DF_Extension)</li>
            <li>Form controls "_FC_" infixed. (i.e. tmsSalesTable[name of control]_FC_Extension)</li>
        </ul>
    </li>
    <li>Event handler classes
        <ul>
            <li>[pre-defined prefix][object name]_EventHandler (i.e. tmxSalesTable_T_EventHandler)</li>
        <ul>
    </li>
</ul>

<br>
<hr>
Link to <a href="https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/dev-ref/xpp-classes-methods">Microsoft documentation</a>