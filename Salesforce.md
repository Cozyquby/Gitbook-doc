
# Salesforce

## Account Integration using Apps and OAuth  

To begin, you will need:  

- A Salesforce account.  

**STEP 1**: In iMBrace, create a new credential of type **Salesforce OAuth2 API**. Copy the URL  
displayed under **OAuth Redirect URL**.  
**STEP 2**: In Salesforce, click on the gear icon in the top-right corner and go to **[Setup]** in the  
dropdown.  
**STEP 3**: In the left side-bar, go to **Platform Tools > [Apps] > [App Manager]**. To create a new app  
to be used with iMBrace, click on **[New Connected App]** near the top-right corner.  
**STEP 4**: Enter the relevant information into the fields as necessary, then enable the checkbox  
**[Enable OAuth Settings]** near the bottom of the screen. Additional options will appear under the  
checkbox.  
**STEP 5**: Paste the redirect URL copied in step 1 into the **Callback URL** field. Under **Selected OAuth  
Scopes**, select the **Full Access** and **Perform requests at any time** scopes.  
**STEP 6**: Save the app settings to create a new app. Resolve any errors and enter any missing  
information as necessary.  
**STEP 7**: The newly-created app should appear in the list of apps under **App Manager**. Click on the  
down-arrow on the right for your app, then click **[View]** in the dropdown that appears.  

> At the time of this document, Salesforce has a bug and this down arrow is not clickable unless you first click on the space or the check mark next to it on the left.  

**STEP 8**: Under the **API (Enable OAuth Settings)** section, go to **[Manage Consumer Details]**.  

> You may be prompted by Salesforce to perform email verification before continuing.  

**STEP 9**: Identify the **consumer key** and **consumer secret**. Copy and paste them into iMBrace  
under the **client ID** and **client secret** fields respectively.  
**STEP 10**: Select the correct **environment type**, and click **[Connect]**.  

**DONE**: The credential can then be used for Salesforce nodes.
