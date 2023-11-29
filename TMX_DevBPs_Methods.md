##Methods

####Considerations
* Methods should be written to encapsulate specific functionality. Smaller methods that target a specific functionality are easier to read and maintain. For instance, do not put the entire function of a SysOperation service class into the run() method or similar entry point. Break apart the various functionalities into methods that call each other in a logical structure.
* Chain-of-command (CoC) methods should be an main entry point for calling the next() method.  Any additional code needed for the extension should be written in a new method or class called from the CoC method.

####Naming conventions
* Methods created directly on an extension object should use the project or initiative prefix.
* The name of the method should clearly define what the function of the method achieves.
* Parameters should be prefixed with an underscore "_".

####Coding standards
* Use camel-case when naming variables: capitalize the first letter of each word or section in the method name and leave the rest of the letter lower-case for readability
* All method code written should be legible and spaced correctly. Your code should be readable like a story; use proper spacing between words and punctuation, indentation and conservative use of blank lines between lines of code.
    * When declaring variable blocks, align the variable names:
    ```C#
    Description             myDesc;
    TransDate               myTransDate;
    AmountCur               myAmount;
    ```
    * When writing code, make sure to indent new sections as they are moved into a new control scope. In this example, the while select and if statement represent control scope changes and the code is indented properly to display this visually:
    ```C#
    SalesTable          salesTable;
    boolean             isOpen = false;

    while select salesTable
    {
        if (salesTable.SalesStatus == SalesStatus::BackOrder)
        {
            isOpen = true;
        }
    }
    ```
    * When writing SQL syntax in the X++ languague, take care to align the conditions of the while/select statement. In this example, each join, where clause and data manipulation are aligned by indent and pushed onto new lines for readability:
    ```C#
    SalesLine               salesLine;
    SalesTable              salesTable;

    select firstOnly SalesStatus, sum(SalesQty) from salesLine
        join salesTable
            where salesLine.SalesId     == salesTable.SalesId       &&
                  salesLine.SalesStatus == SalesStatus::Backorder   &&
                  salesTable.SalesId    == 'SO00000001'
        group by salesLine.SalesStatus;
    ```
* Avoid the use of the 'var' keyword when coding and opt for the type of the object. Along the same lines, avoid the use of the base types when naming variables and use the most logical extended data type.
* Static text should be assigned a label and wrapped in double-quotes wherever possible. Thinkmax are usually involved in projects where English and French are used at a minimum and labels standardize translations.
    * Where labels cannot be used or are not applicable, put static text inside single-quotes.

---
Link to [Microsoft documentation](https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/dev-ref/xpp-language-reference)
