
# monday.com

monday.com provides two methods to integrate with iMBrace: OAuth tokens and personal API  
tokens. OAuth tokens provide more fine-grained control over the permissions that are granted to  
external apps like iMBrace. The following instructions show how to integrate monday.com with  
iMBrace using either method.

## Account integration using API token  

You will need:  

- A monday.com account to integrate with iMBrace
- A monday.com user with access to the above account (admin access is **not** required)

> For more information, you may refer to the official [monday Developers documentation](https://developer.monday.com/api-reference/docs/authentication).  

**STEP 1**: Open the drop-down menu in the top-right corner, then go to **Account > [Developers]**.  
**STEP 2**: In the left side-bar, go to **[My access tokens]**.  
**STEP 3**: You will be able to access your API token here. Copy the token by clicking **[Show]**, then  
clicking **[Copy]**.  
**STEP 4**: In iMBrace, create a new credential of type **Monday.Com API**, paste the copied token into  
the **Token V2** field, then click **[Create]**.

**DONE**: The credential can then be used for **Monday.com** nodes.

## Account integration using OAuth  

You will need:  

- A monday.com account to integrate with iMBrace  
- A monday.com user with access to the above account (admin access is **not** required)  

> For more information, you may refer to the official [monday Developers documentation](https://developer.monday.com/api-reference/docs/authentication).

**STEP 1**: Open the drop-down menu in the top-right corner, then go to **Account > [Developers]**.  
**STEP 2**: In the left side-bar, go to **[My apps]**. Then click **[Build app]** or **[Create app]**.  
**STEP 3**: Fill in the relevant information for your new app. Finish creating the app by clicking **[Save  
App]** at the bottom.  
**STEP 4**: Under App Credentials, identify the **client ID** and **client secret**. You can view the secret by  
clicking **[Show]**, and you can copy the ID and secret by clicking **[Copy]**.  
**STEP 5**: In iMBrace, create a new credential of type **Monday.Com OAuth2 API** and paste the  
copied client ID and client secret into their respective fields. Also identify and copy the **OAuth  
Redirect URL**. You can copy the redirect URL by clicking **[Copy URL]**.  
**STEP 6**: In the monday Developer Center, go to **[OAuth]** in the left side-bar.  
**STEP 7**: Under the **Scopes** tab, select the boards:read and boards:write scopes.  
**STEP 8**: Under the **Redirect URLs** tab, paste the copied redirect URL from step 5 into the **Redirect  
URLs** field. Then click **[Save Feature]** at the bottom.  
**STEP 9**: In iMBrace, finish creating the credential by clicking **[Connect]**.  

**DONE**: The credential can then be used for **Monday.com** nodes.
