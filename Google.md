
# Google

### Gmail, Google Drive, Docs, Sheets, Calendar, etc.  

Google provides a standardized way to access their APIs through the Google Cloud Console. This  
can be done using OAuth (for per-user access) or service accounts (for per-service access). Once  
configured, you can use your credentials to authenticate the following nodes:  

## Google compatible nodes  

## Account integration using OAuth  

To begin, you will need:  

- A Google account.
- A Google Cloud Platform project for use with iMBrace.  

**STEP 1**: Go to [Google Cloud Console](https://console.cloud.google.com).  
**STEP 2**: Navigate to the correct project in the top-left corner. Create a new project if necessary.  
This can be done by navigating to **[Projects]** and selecting **[New Project]**.  
**STEP 3**: In the left side-bar, go to **[APIs & Services] > [Credentials]**.  
**STEP 4**: Go to **[Create Credentials] > [OAuth client ID]**.  
**STEP 5**: If you are creating an OAuth ID for the first time, you will need to configure a **consent  
screen** as well. For more detailed information, see the following [Google help page](https://support.google.com/cloud/answer/10311615?hl=en&ref_topic=3473162).  

Note: Remember to **Publish App** to **In production**.  

- Enter **App information** 
- Enter **Authorized domains**: "imbrace.co" and **Developer contact information**
- **PUBLISH APP** to **In Production**

**STEP 6**: In the left side-bar, go to **Enabled APIs & services** and click **+ ENABLE APIS AND**  
**SERVICES** to enable the Google services you need.

Search the relevant APIs to be used (For example, Google Docs API, Google Sheets, etc.) and click  
**Enable**.  

**STEP 7**: In iMBrace, create a new credential and select a integration (Google Docs OAuth2 API,  
Google Sheets OAuth2 Api, etc.), copy the **OAuth Redirect URL**.  
**STEP 8**: In Google Cloud Console, go to Credentials > +CREATE CREDENTIAL > OAuth client ID,  
enter the information and paste the **OAuth Redirect URL** under **Authorized redirect URIs** to create  
an OAuth client ID.  
**STEP 9**: You will then be presented with the **client ID** and **client secret** for the OAuth client.  
**STEP 10**: In iMBrace, paste the **Client ID** and **Client secret** into the corresponding fields. Then click  
**CONNECT** to complete the authentication.

Follow the pop-up window to login to Google account and complete the authentication.

**DONE**: You can see the connected message, the credential can then be used for Google integrations..
