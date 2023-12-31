#Thinkmax development best practices
##Introduction

The contents of this wiki and its subcomponents are meant to guide D365F&O development at Thinkmax and provide a framework for both developers and dev leads in the process of performing development and code reviews.

By no means are the directives in this best practice guide the "law" and the final decision on best practices on an implementation are made by the dev lead on the project. We believe that the guidelines in this wiki will help standardize development and streamline developers as they move between implementation projects.

The naming conventions suggested in this document are highly recommended, but could change due to a client constraint or project decision.
Microsoft uses module and entity prefixes on their objects to define what part of the application refers to (i.e. CustCustomer, InventoryTrans, Retail, etc...). It is recommended that custom tables developed follow the same naming convention where applicable. For instance a class name like TMXUpdateShipDateRequested isn't as specific as TMXSalesUpdateShipDateRequested or TMXWHSWorkUpdateShipDateRequested.

All object naming, both in code and the AOT, will use <b><i>camel casing</i></b> (i.e. ThinkmaxDevelopmentStandards)

</br>
If you ever have any questions on the contents of this wiki, or wish to suggest a change, please email TEC@thinkmax.com.

###Table of contents
- [Extended data types](TMX_DevBPs_EDTs.md)
- [Enums](TMX_DevBPs_Enums.md)
- [Tables](TMX_DevBPs_Tables.md)
- [Views](TMX_DevBPs_Views.md)
- [Queries](TMX_DevBPs_Queries.md)
- [Data entities](TMX_DevBPs_DataEntities.md)
- [Forms](TMX_DevBPs_Forms.md)
- [Classes](TMX_DevBPs_Classes.md)
- [Methods](TMX_DevBPs_Methods.md)
- [Labels](TMX_DevBPs_Labels.md)
- [Security](TMX_DevBPs_Security.md)
- [Code review policies](TMX_Dev_CodeReviewPolicies.md)
- [Check-in policies](TMX_Dev_CheckInPolicies.md)