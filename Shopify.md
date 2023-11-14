
# Shopify 

Shopify offers developers to integrate Shopify's functionality into custom apps outside of the  
official website. This can be used to allow access to Shopify's API through the iMBrace platform.  

## Account integration using Apps  

To begin, you will need:  

- A Shopify account with an associated online storefront.  

**STEP 1**: In the bottom-left corner, go to **[Settings]**.  
**STEP 2**: In the left side-bar, go to **[Apps and sales channels]**.  
**STEP 3**: Go to **[Develop apps for your store] > [Allow custom app development]**.  
**STEP 4**: Once enabled, create a new app and enter the necessary information in the dialog box  
that appears.  
**STEP 5**: Go to **[Configuration] > [Admin API integration]**. Select the relevant access scopes for  
use with the iMBrace platform.  
**STEP 6**: In the top-right corner, click on **[Install App]** to generate access tokens.  
**STEP 7**: You will then be able to view your **API key, secret key** and **access token** for your Shopify  
app.  
**STEP 8**: Identify the **subdomain** of your Shopify storefront. This is the part of the URL before the  
“**.myshopify.com**” (in the example below, it is “f337c7”).  
**STEP 9**: In iMBrace, create a new credential of type **Shopify API** and enter the API key and shop  
subdomain. Enter the secret key into the **Shared Secret** field and the access token into the  
**Password** field. Then click **[Submit]**.  

**DONE**: The credential can then be used with Shopify nodes.
