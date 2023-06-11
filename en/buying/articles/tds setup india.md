## TDS Setup for India

To setup **_TDS_** in ERPNext follow below steps:

*   First you have to define Tax withholding categories, by default 28 categories are already pre-defined as per Indian statutory compliances. But if you want to add new category then you can create the same by clicking on "New"(button at right top corner)

![](https://docs.erpnext.com/files/Oq1mP48.png)

*   As per category you have to define Tax withholding rate along with "Single Transaction Threshold" & "Cumulative Transaction Threshold" for Financial/Fiscal year.

![](https://docs.erpnext.com/files/MELGDIu.png)

*   In same screen you will find another section of "Account Detail" to set company-wise TDS Payable account.

![](https://docs.erpnext.com/files/IIB6N8R.png)

*   Once you are done with Tax withholding setup go to Supplier master and assign Tax withholding category.

![](https://docs.erpnext.com/files/aThoNuR.png)

*   Now when you create a Purchase invoice against that supplier make sure "Apply Tax withholding Amount" is checked then only system will auto fetch TDS Payable amount in "Taxes & Charges" table based on Threshold you have defined.

![](https://docs.erpnext.com/files/zyZdwsr.png)

![](https://docs.erpnext.com/files/XUJEgQ7.png)

Standard report is also available to check monthly payable, just search for "TDS payable monthly" report for the same.