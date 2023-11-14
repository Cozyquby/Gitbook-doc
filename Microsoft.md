
# Microsoft 

### Microsoft Outlook, Teams, OneDrive, Excel, etc.  

Microsoft provides a standardized way to access their APIs through Microsoft Azure. This can be  
done using **OAuth**. Once configured, you can use your credentials to authenticate the following  
nodes:  

## Microsoft compatible nodes

| Node                      | OAuth |
| :-------------------------| ------|
| Microsoft Dynamics CRM    | Yes   |
| Microsoft Excel           | Yes   |
| Microsoft Graph Security  | Yes   |
| Microsoft OneDrive        | Yes   |
| Microsoft Outlook         | Yes   |
| Microsoft Teams           | Yes   |
| Microsoft To Do           | Yes   |  

## Account integration using OAuth  

To begin, you will need:  

- An [Microsoft Azure](https://azure.microsoft.com) account.

**STEP 1**: Access the [Microsoft Application Registration Portal](https://aka.ms/appregistrations).  
**STEP 2**: Click on the **[Register an application]** button.  
**STEP 3**: Enter a name for your app in the **Name** field.  
**STEP 4**: Select **Accounts in any organizational directory (Any Azure AD directory - Multitenant)  
and personal Microsoft accounts (eg. Skype, Xbox)** under the **Supported account types** section.  
**STEP 5**: In iMBrace, copy the **OAuth Callback URL** provided in the Microsoft node credentials.  
**STEP 6**: Paste it in the **Redirect URI (optional)** field on the **Register an application** page.  
**STEP 7**: Click on the **[Register]** button.  
**STEP 8**: Copy the **Application (client) ID**.  
**STEP 9**: In iMBrace, enter the name for your credentials in the **Credentials Name** field in  
the Microsoft node credentials (In this case, Microsoft Outlook).  
**STEP 10**: In iMBrace, paste the Application ID in the **Client ID** field in the Microsoft node  
credentials.  
**STEP 11**: On your Microsoft application page, click on **[Certificates & secrets]** in the left sidebar.  
**STEP 12**: Click on the **[+ New client secret]** button under the **Client secrets** section.  
**STEP 13**: Enter a description in the **Description** field.  
**STEP 14**: Click on the **[Add]** button.  
**STEP 15**: Copy the displayed secret under the **Value** column.  
**STEP 16**: In iMBrace, paste the secret in the **Client Secret** field in the Microsoft node credentials.  
**STEP 17**: Click on the **[Connect]** button in the OAuth section to connect a Microsoft account to  
iMBrace.  
**STEP 18**: Login to your Microsoft account and allow the app to access your info.  
**STEP 19**: In iMBrace, click on the **[Save]** button in the Microsoft node credentials to save your  
credentials.  

**DONE**: The credential can then be used for Microsoft nodes.
