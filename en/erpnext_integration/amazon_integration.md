## Amazon SP-API Integration

The Amazon Connector pulls Products and Sales Orders from Amazon marketplace. The sync of Products and Sales Orders is sequential. You have to sync the products before you Sync the Sales Orders.

## How to Setup Amazon SP-API Connector?

Amazon Connector is moved out from ERPNext and available through a Frappe App on [Frappe Cloud Marketplace](https://frappecloud.com/marketplace/apps/ecommerce_integrations)

### App Installation

*   If you are hosting your ERPNext site on Frappe Cloud, you can quickly install the app by going to your site Dashboard. The app is available in [Frappe Cloud Marketplace](https://frappecloud.com/marketplace/apps/ecommerce_integrations)
*   If your site is hosted by Frappe, please raise a support ticket to get the app installed on your site.
*   If you are self hosting ERPNext you can install the app using Frappe bench. Refer [bench documentation](https://frappeframework.com/docs/user/en/bench/frappe-commands#app-installation) for installing Frappe Apps. `bench get-app ecommerce_integrations --branch main`

The repository for app is hosted on GitHub: [http://github.com/frappe/ecommerce\_integrations/](http://github.com/frappe/ecommerce_integrations/)

### Setting Up Credentials in ERPNext

You can request the developer credentials from Amazon SP once you are a registered seller on their website. For more details on the same, click [here](https://developer.amazonservices.com/).

#### 1\. Setup SP-API Credentials

Enter the IAM ARN, Refresh Token, Client ID, Client Secret, AWS Access Key, AWS Secret Key and Country. ![Setup Credentials](https://docs.erpnext.com/files/amazon_sp_api_settings_1..png)

#### 2\. Set up Order Details

Set up Company, Warehouse, Parent Item Group, Price List, Customer Group, Territory, Customer Type and Account Group. The Account Group is used to hold Commission, taxes etc. that Amazon charges. ![ERPNext Configurations](https://docs.erpnext.com/files/amazon_sp_api_settings_2..png)

#### 3\. Setup Sync Configurations

Using the After Date, you can sync products and orders created after a particular date. In case you are importing a lot of historic data, it is suggested to start in the reverse chronological order of the After Date and import data in small chunks. ![Sync Configurations](https://docs.erpnext.com/files/amazon_sp_api_settings_3..png) After setting up all the configurations, click on Enable Amazon and save the settings. You are now ready to use the integration.

#### 4\. Sync Products

Click on this button to sync products. Once this is successful you should see your Amazon products as Items in ERPNext.

![Sync Configurations](https://docs.erpnext.com/files/amazon_mws_settings_4.png) ![Sync Configurations](https://docs.erpnext.com/files/amazon_mws_settings_5.png)

#### 5\. Sync Orders

Click on this button to sync sales orders. Once this is successful you should see your Amazon Orders as Sales Orders in ERPNext. You can also set up scheduler to sync orders automatically.

> In case your developer account does not have access to personally identifiable information. The customer name would be stored as a combination of the BuyerName + <Order ID>.

![Sync Configurations](https://docs.erpnext.com/files/amazon_mws_settings_6.png)

### Note

The connector won't handle Order cancellation. If you cancelled any order in Amazon then manually you have to cancel respective Sales Order and other documents in ERPNext.