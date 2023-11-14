
# ServiceNow

**ServiceNow**  

[ServiceNow](https://developer.servicenow.com/dev.do) is a cloud computing platform to help companies manage digital workflows for their  
operations.  

**Account integration using OAuth**

To begin, you will need:  

- A [ServiceNow](https://developer.servicenow.com/dev.do) account.

**STEP 1**: Register an account, click on **[Start building]**.  
**STEP 2**: Click on **[Request Instance]**.  
**STEP 3**: Login with the given username and password.  
**STEP 4**: Navigate to **System OAuth > Application Registry**.  
**STEP 5**: Click **[New]** button > **Create an OAuth API endpoint for external clients**.  
**STEP 6**: Complete the following fields:  

- **Name**: Enter a descriptive name for the new endpoint.
- **Client ID**: Auto populated field, you will need this ID to configure your **iMBRACE** credentials.
- **Client Secret**: Enter your desired secret or leave **blank** to auto generate a random string. You  
  will need this to configure your credentials.
- **Redirect URL**: In iMBRACE, copy the **OAuth Callback URL**.
  - iMBRACE
  - Paste it in ServiceNow.

**STEP 7**: Click **[Submit]** to save and create your new endpoint.  
**STEP 8**: In iMBrace, enter a descriptive **Credentials Name**.  
**STEP 9**: Under **Credential Data** complete the following fields:   

- **Client ID**: Enter the client ID generated above.
- **Client Secret**: Enter your client secret created above.
- **Subdomain**: Enter the subdomain of your ServiceNow instance. This can be seen in your  
  instance URL: **https://<subdomain>.service-now.com/**.

**STEP 10**: From the **OAuth** section, click the **[Connect button]** to establish the connection and  
finalize your iMBRACE credentials.  

**DONE**: The credential can then be used for ServiceNow nodes.
