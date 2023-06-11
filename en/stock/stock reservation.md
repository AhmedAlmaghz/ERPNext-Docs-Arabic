## Stock Reservation

> Introduced in Version 15

Stock reservation, also known as inventory reservation, refers to the practice of setting aside a specific quantity of stock or inventory for a particular purpose or customer.

### 1\. Prerequisites

*   Enable Stock Reservation in Stock Settings. ![stock reservation settings5cee61](https://docs.erpnext.com/files/stock-reservation-settings5cee61.png)

### 2\. Stock Reservation against Sales Order

*   Create a Sales Order. ![sales order9407a4](https://docs.erpnext.com/files/sales-order9407a4.png)
    
*   Check the reserve stock for items you want to reserve. ![reserve stock checkbox100a2c](https://docs.erpnext.com/files/reserve-stock-checkbox100a2c.png)
    
*   Click on **Stock Reservation**, then select **Reserve**. Choose the warehouse and quantity, and finally, click on the **Reserve Stock** button. ![reserve stock demobe5804](https://docs.erpnext.com/files/reserve-stock-demobe5804.gif)
    
*   Stock reservation entries are created against the sales order items. ![stock reservation entriesef4510](https://docs.erpnext.com/files/stock-reservation-entriesef4510.gif)
    

### 3\. Stock Unreservation

There are two ways to unreserve the stock.

1.  Stock Unreservation from Sales Order:
    
    *   Open a Sales Order and click on **Stock Reservation > Unreserve** button, the Stock Reservation Entries gets cancelled. ![unreserve stock from sales order](https://docs.erpnext.com/files/unreserve-stock-from-sales-order.gif)
2.  Unreserve the stock from the Stock Reservation Entry DocType:
    
    *   2.1 Open a Stock Reservation Entry and cancel it by clicking the **Cancel** button. ![cancel sre](https://docs.erpnext.com/files/cancel-sre.gif)
        
    *   2.2 Go to the Stock Reservation Entry List, select the entries you wish to cancel, and then click on **Actions > Cancel**. ![bulk cancel sre](https://docs.erpnext.com/files/bulk-cancel-sre.gif)
        

1.  [Sales Order](https://docs.erpnext.com/docs/v14/user/manual/en/selling/sales-order)