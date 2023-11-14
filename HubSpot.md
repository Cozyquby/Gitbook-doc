
# HubSpot

HubSpot provides multiple ways to integrate functionality with their system, including API keys,  
Ecommerce Bridge and Private Apps. The following instructions show how to integrate with  
HubSpot using Private Apps (which replace API keys).  

## Account integration using Private Apps  

To begin, you will need:  

- A HubSpot account.  

**STEP 1**: In the top-right corner, go to your account's **[Profile & Preferences]**.  
**STEP 2**: In the left side-bar, go to **[Account Setup] > [Integrations] > [Private Apps]**.  
**STEP 3**: Create a new private app and fill in the name, logo and description for the app.  
**STEP 4**: Select the scopes that are necessary for the required functionality. A full list of the scopes  
used by HubSpot-related nodes can be found [below](https://imbrace.gitbook.io/imbrace-no-code-workflow/integrations/hubspot#hubspot-scopes).  
**STEP 5**: In the top-right corner, click **[Create App]** to generate an **access token**. After creation,  
you can view and copy the token.  
**STEP 6**: In iMBrace, create a new credential of type **HubSpot App Token** and enter the access  
token. Then click **[Submit]**.

**DONE**: The credential can then be used for HubSpot nodes.  

## HubSpot scopes  

Credentials for HubSpot-related nodes should have the following scopes:  

**HubSpot node**:  

- oauth
- crm.objects.companies.read
- crm.objects.companies.write
- crm.objects.contacts.read
- crm.objects.contacts.write
- crm.objects.deals.read
- crm.objects.deals.write
- crm.objects.owners.read
- crm.schemas.companies.read
- crm.schemas.contacts.read
- crm.schemas.deals.read
- forms
- tickets  

**HubSpot Trigger node**:  

- oauth
- crm.objects.companies.read
- crm.objects.contacts.read
- crm.objects.deals.read
- crm.schemas.companies.read
- crm.schemas.contacts.read
- crm.schemas.deals.read
