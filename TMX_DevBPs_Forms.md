##Forms

####Considerations
* In the vast majority of cases, a pattern should be chosen from the <a href="https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/user-interface/user-interface-development-home-page#form-pattern-guidelines">pre-defined list</a> available on the form design. These pre-defined patterns standardize form development and guide the developer to include relevant form controls with appropriate settings for the pattern chosen.  Only in fringe cases where the form design cannot flexibly fit into the pre-defined patterns should the “Custom” pattern be used.
* There will not be many “standards” for form development as the options and permutations available are many  In general when developing forms, keep in mind the user experience and usability of the form. Form navigation should be clean and concise, with controls and grid columns labeled clearly and appropriately.
* When writing code for form extensions, refer to the coding standards guidelines for using CoC methods in extension classes and event handler classes.

####Naming conventions
* Form controls added to forms via extension should be named with the project or initiative prefix.
* There are no specific Thinkmax guidelines for form naming conventions. Typically forms are named after the table that the form exposes the data for, or they summarize the function of the various data sources interacting with the form.  Refer to the naming convention notes in the Introduction for more general details.

####Required object properties
|Type|Required property|Value|
|:-|:-|:-|
|Design|Caption||
|FormDataSource|Table||
||Allow Create||
||Allow Delete||
||Allow Edit||
||Insert At End||
||Insert If Empty||
||Join Source||
|FormTabPageControl|Caption||
|FormQuickFilter|Default Column||
||Target Control||
|FormButtonGroup|Caption||
|FormMenuFunctionButtonControl|Menu Item Type||
||Menu Item Name||
|FormButtonControl|Text||
|FormControl|Data Source||
||Data Field <br><i>If control data comes from data source field</i>||
||Data Method <br><i>If control data comes from data source method</i>||
|FormStaticText|Text||

<hr>
Link to <a href="https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/user-interface/user-interface-development-home-page">Microsoft documentation</a>