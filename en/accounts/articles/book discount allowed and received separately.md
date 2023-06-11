Discounts are part of everyday businesses. A discount allowed is when the supplier of goods or services grants a payment discount to a customer. On the other hand, a discount received is the reverse situation, where the customer is granted a discount by the supplier.

When you are a supplier, and you grant a discount to your customer, it is treated as a type of Expense, whereas, if you receive a discount from your supplier, it is considered as an income.

In ERPNext, discount allowed or received is not booked separately. It is typically the final amount of the invoice (after discount) that is booked. However, if you wish to book the discounts separately, you can follow the below steps:

1) "Discount Allowed" is a type of Expense and "Discount Received" is a type of Income. Hence, first create these two accounts in the Chart of Accounts.

![](https://docs.erpnext.com/files/tE7sKIX.png)

2) Create an invoice, select the item. Now, under the "Sales/Purchase Taxes and Charges" table, select the discount account head depending on the transaction, and enter the discount rate as a negative value.

For example, if we are creating a Sales Invoice, and we are giving a discount of 10% to the customer, the 10% discount is booked in a separate "Discount Allowed" account. Check the screenshot below to understand the same.

![](https://docs.erpnext.com/files/8QtX0DE.jpe)

As seen in the screenshot above, the total value of the invoice without discount is Rs. 350. On applying 10% discount, the total value of the invoice now comes down to Rs. 315. The discount amount of Rs. 35 is booked under the Discount Allowed account which is a type of expense for the supplier. Check the below screenshot to understand how the accounts are booked.

![](https://docs.erpnext.com/files/IMAGE%202020-11-18%2011:45:41.jpg)

3) Proceed to making the final payment via Payment Entry as shown in the screenshots below:

![](https://docs.erpnext.com/files/18fssIO.png)

![](https://docs.erpnext.com/files/rDzKNPb.png)

**Note:** The same process can be followed while creating a Purchase Invoice. However in this case, the account selected in the Purchase Taxes and Charges table will be "Discount Received" which will be an income account.