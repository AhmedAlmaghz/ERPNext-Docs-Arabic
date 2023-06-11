## Routing

**Routing is a template of BOM Operations.**

A Routing stores all Operations along with the description, hourly rate, operation time, batch size, etc. Creating a Routing for your BOM Operations is useful when similar Operations are used for manufacturing different items.

To access the Routing list, go to:

> Home > Manufacturing > Bill of Materials > Routing

## 1\. Prerequisites

*   [Operation](https://docs.erpnext.com/docs/v13/user/manual/en/manufacturing/operation)
*   [Workstation](https://docs.erpnext.com/docs/v13/user/manual/en/manufacturing/workstation)

## 2\. How to Create a Routing

1.  Go to the Routing list, click on New.
2.  Enter a name for the Routing.
3.  Enter the Operations in the BOM Operation table:
    1.  Select the Operation.
    2.  The default Workstation will be fetched.
    3.  Enter the Hourly Rate for running this Operation.
    4.  Enter the Operation Time in minutes.
    5.  Enter the Batch Size, i.e. the number of units processed in this Operation.
    6.  The Operating Cost will be calculated based on the Hourly Rate and the Operation Time.
4.  Save.
    
    ![Routing](https://docs.erpnext.com/files/routing.png)
    

Once created, a Routing can be selected in a BOM to fetch the Operations stored in the Routing. ![Routing BOM](https://docs.erpnext.com/files/routing-bom.png)

## 3\. Sequence ID in Routing

![Routing Sequence ID](https://docs.erpnext.com/files/sequence-id-routing.png) Sequence ID enforces the users to complete the operations sequentially via Job Card. In case a user tries to complete an operation before completing any of its precedent operations as per the Sequence ID, the system throws a validation error.

1.  [Work Order](https://docs.erpnext.com/docs/v13/user/manual/en/manufacturing/work-order)
2.  [Bill Of Materials](https://docs.erpnext.com/docs/v13/user/manual/en/manufacturing/bill-of-materials)