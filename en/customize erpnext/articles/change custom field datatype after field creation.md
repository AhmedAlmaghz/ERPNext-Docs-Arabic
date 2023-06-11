On creation of a custom field, it is not possible to change datatype directly once the form is updated. To understand how to fix this issue, let's take an example.

Let's assume, we have created a custom field called "Client" in some DocType, and have set the datatype of the field to "Data" and have updated the form.

![](https://docs.erpnext.com/files/oC1x4VU.png)

But we wish to change the field from Data to Link as shown below.

![](https://docs.erpnext.com/files/ipJDZu3.png)

However on doing so, when we click on update, an error is thrown as shown in the screenshot below.

![](https://docs.erpnext.com/files/j6CBjuB.png)

To fix this, navigate to Custom Field list via the search bar. Search for the field whose datatype you wish to change.

![](https://docs.erpnext.com/files/BzHBToc.png)

Open the record and change the datatype. Make sure to enter any other relevant information too. In this case, the "Options" field needs to be filled if we want to change the datatype to "Link". Click on Save.

![](https://docs.erpnext.com/files/feW55Of.png)

Now, go back to Customize Form and check the field. It should be changed to the new datatype.

![](https://docs.erpnext.com/files/K9EkoHp.png)