## Google Contacts Integration

ERPNext provides an integration with Google Contacts in order for all users to synchronize their Google Contacts with ERPNext.

In order to allow a synchronization with Google Contacts, you need to authorize ERPNext to get Contacts data from Google. Google Contacts Integration is set up with the following steps:

*   Create OAuth 2.0 Credentials via [Google Settings](https://docs.erpnext.com/docs/v13/user/manual/en/erpnext_integration/google_settings).
*   In the Google Contacts list, click on New. Enter the Google Account Email you want to sync and then save it. Now click on **Authorize Contacts Access** to authorize ERPNext to get Contacts data from Google.

### Creating a Contacts in ERPNext

*   Once Google Contacts Integration is succesful, all the contacts created in ERPNext will be synced if `Push to Google Contacts` is checked.

Creating a Contact in ERPNext: ![](https://docs.erpnext.com/files/google_contacts_create_contact.gif)

It will be shown in Google Contacts: ![](https://docs.erpnext.com/files/google_contacts_create_contact_!.gif)

### Syncing Contacts from Google Contacts

*   Once Google Contacts Integration is succesful, all the contacts in Google Contacts will be synced if `Pull from Google Contacts` is checked. ![](https://docs.erpnext.com/files/google_contacts_contact_sync.gif)