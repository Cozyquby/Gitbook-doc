
# Freshworks CRM

Freshworks CRM can be integrated into the iMBrace platform using an API key for a given user  
account.  

## Account integration using API key  

To begin, you will need:  

- A Freshworks CRM account.  

**STEP 1**: In the top-right corner, go to the account’s **[Settings] > [API Settings]**. You may need to  
complete a CAPTCHA to access API settings.  
**STEP 2**: Copy the **API key** and identify the **subdomain** (the portion of the **bundle alias** before  
“**.freshworks.com**” (in the example below, it is “imbrace-514705880258403489”.)  
**STEP 3**: In iMBrace, create a new credential of type **Freshworks CRM API** and enter the API key.  
Enter the subdomain in the **Domain** field. Then click **[Submit]**.  

**DONE**: The credential can then be used for Freshworks CRM nodes.
