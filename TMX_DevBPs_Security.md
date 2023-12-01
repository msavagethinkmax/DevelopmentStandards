##Security objects

####Considerations
* Thinkmax best practices for security objects will have developers expose access points as privileges as part of their FDD deliverables where security development is relevent.  This allows end-users to configure security on the UI side of the application (System administration > Security > Security configuration).  Unless stated in the FDD, no additional development should be done. 
* Privileges
  * In all cases for form access, a privilege should be created for read-only access. If applicable, a separate privilege should be created for access to edit the backing data.

####Naming conventions
* Privileges
  * When access level is "Read", object name should end in "View".
  * When access level is "Correct" or "Delete", object name should in in "Maintain".

####Required object properties
|Type|Required property|Default value|
|:-|-|-|
|Privilege|Label||
|Privilege entry point|Object type||
||Object name||
||Access level||
|Privilege data entity permission|Grant||
|Policy|Context type||
||Label||
||Query||
||Primary table||
||Operation||

---
Link to [Microsoft documentation](https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/sysadmin/security-architecture)