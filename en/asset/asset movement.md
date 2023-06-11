## Asset Movement

**Asset Movement refers to moving an Asset from one Location to another.**

In ERPNext, you can track the location of an asset or to whom it is issued. For tracking, you need to create an Asset Movement transaction, whenever the asset is moved from one location to another. You can also keep a track of issuance of an asset to any employee.

To access the Asset Movement list, go to:

> Home > Assets > Assets > Asset Movement

![Asset Movement](https://docs.erpnext.com/files/asset-movement.png)

## 1\. Prerequisites

Before creating and using Asset Movement, it is advised to create the following first:

*   [Asset](https://docs.erpnext.com/docs/v13/user/manual/en/asset/asset)
*   [Asset Location](https://docs.erpnext.com/docs/v13/user/manual/en/asset/asset-location)

## 2\. How to create an Asset Movement

1.  Go to the Asset Movement list, click on New.
2.  Select the Purpose from 'Issue', 'Receipt', or 'Transfer'. Mandatory fields will be changed based on purpose.
3.  Select a date.
4.  Select Assets you want to move. Current Location / Custodian will be automatically fetched.
5.  Select Reference Document Type (Optional).
6.  Select Reference Document Name (Optional).
7.  Save.
8.  Submit.

To make an Asset Movement of a number of assets, it is advised to go to Asset List, select assets to be moved and click on **Make Asset Movement** from Actions menu on the top left.

![Move Multiple Assets](https://docs.erpnext.com/files/asset-movement-using-button.png)

There is also a **Transfer Asset** button on the top right of the Asset form to initiate Asset Movement. It auto fills available fields from Asset Form.

![Move Single Asset](https://docs.erpnext.com/files/asset-movement-using-transfer-asset-button.png)