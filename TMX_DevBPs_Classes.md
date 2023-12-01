##Classes

####Considerations
* Classes are created by developers to contain code in methods to perform a necessary function.
* Practice **encapsulation** when developing your classes and structures.  Classes should be created for a specific functionality.  Do not group multiple functionalities in the same class
* Be very mindful of the amount and reusability of your code.  If a functionality varies slightly from case to case, see if you can write a dynamic method to handle the variations, rather than writing multiple methods.<br>The same approach would apply to creating class structures. If you can create a base class to do the core function and create extension classes to handle the variations, this is preferable rather than having redundant objects and code.
  * The consideration of this point is important to the code review process.  
* Extension classes
  * For project development, it is optimal to have one extension class per object per model.
* Event handler classes
  * Follow Microsoft recommendation: opt for using a CoC method extension rather than an event handler.  Do not create an OnInserting table event handler method, extend the insert() method on a table.
  * Do **not** mix event handler methods across different objects in the same event handler class. All event handler methods in the event handler class should relate back to a single object.

####Naming conventions
* Use camel-case in object naming
* Prefix **ALL** class names with the pre-defined project or initiative abbreviation (i.e. Thinkmax Vertical object names begin with "tmx").
* Make **meaningful** names for classes.
  * The name of a class is important and should accurately detail the purpose of the class.
  * possible include the module and entity in the object name to define what area of the product it relates to (i.e. 'TMS', 'WHS', 'Sales', 'Invent', etc.)
* Extension classes
  * Table extension methods have "_T_" infixed. (i.e. tmxSalesTable_T_Extension)
  * Form extension classes have "_F_" infixed. (i.e. tmxSalesTable_F_Extension)
  * Form data sources have "_FDS_" infixed (i.e. tmxSalesTableSalesLine_FDS_Extension)
  * Form data source data fields have "_DF_" infixed (i.e. tmxSalesTableSalesLineSalesPrice_DF_Extension)
  * Form controls "_FC_" infixed. (i.e. tmsSalesTable[name of control]_FC_Extension)<
* Event handler classes
  * [pre-defined prefix][object name]_EventHandler (i.e. tmxSalesTable_T_EventHandler)

---
Link to [Microsoft documentation](https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/dev-ref/xpp-classes-methods)