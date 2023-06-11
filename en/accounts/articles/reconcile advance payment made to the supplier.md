**While migrating from _x_ application to ERPNext, how to book advance Accounts Payable and reconcile with future invoices?**

**Booking Advance Accounts Payable:**

Create a **Journal Entry** with type **Opening Entry**, Debit the _Creditor Account_ choosing the required _Supplier_ and Credit the _Temporary Opening Account_.

Expand the Creditor's Row and select **Yes** for _Is Advance._

_Refer to the GIF illustrating the same:_

![](https://docs.erpnext.com/files/CsMRH40.gif)

Submitting the Journal Entry will reflect a negative balance in **Accounts Payable Summary**:![](https://docs.erpnext.com/files/FJeIj5k.png)**Reconciling it with the Purchase Invoices:**

Refer to **Accounts Payable** report _after_ creating a Purchase Invoice:

![](https://docs.erpnext.com/files/cxZArKd.png)

Currently, they are not reconciled and are reflected as **two** **separate entries**, use the **Payment Reconciliation** tool to reconcile these both entries, _refer to the GIF for the steps:_

![](https://docs.erpnext.com/files/jbj6LRc.gif)

Refer to Accounts Payable Report after reconciling, it _won't_ reflect the **Journal Entry** anymore and will reflect the (_Invoiced Amount - Advance Amount)_:

![](https://docs.erpnext.com/files/vaXYQNc.png)