#Thinkmax development best practices:
##Security objects

####Considerations
<ul>
    <li>Thinkmax best practices for security objects will have developers expose access points as privileges as part of their FDD deliverables where security development is relevent.  This allows end-users to configure security on the UI side of the application (System administration > Security > Security configuration).  Unless stated in the FDD, no additional development should be done. </li>
    <li>Privileges</li>
        <ul>
            <li>All cases for form access, a privilege should be created for read-only access. If applicable, a separate privilege should be created for access to edit the backing data.</li>
        </ul>
</ul>

####Naming conventions
<ul>
    <li>Privileges</li>
    <ul>
        <li>When access level is "Read", object name should end in "View".</li>
        <li>When access level is "Correct" or "Delete", object name should in in Maintain</li>
    </ul>
</ul>

####Required object properties
|Type|Required property|Value|
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

Link to <a href="https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/sysadmin/security-architecture">Microsoft documentation</a>