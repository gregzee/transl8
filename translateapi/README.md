# Translate API

## Getting Started

You can either go with an API Key or use an OAuth2 workflow. For Transl8, I used OAuth2. If you want to 
with an API Key, you can follow this guide, it's relatively similar."

- [API Key doc](https://translatepress.com/docs/automatic-translation/generate-google-api-key/)
  - Anything related to Translatepress can be excluded.

## Cloud Translate API via OAuth (Setting up)

1. https://console.cloud.google.com/
2.  Make sure you are in the account you want to work in (top right corner)
3. Top left corner, create a new project that is specific to the project
4. In the search bar, search API & Services
5. Enable API Services

  Example:
![image](https://user-images.githubusercontent.com/38545800/156888389-975d8a88-a6d2-4f54-ade7-d178915c8157.png)

## Enable Translation API & Billing

1. Search for Cloud Translation API
2. Enable Cloud Translation API
3. You will need to put in billing information. Review this.
  -  If its your first time using GCP, you should get a 300 dollars credit
  - 500k Characters translated are free. Each 1 million are $20 USD
  - Please review.

**If you are all set up on billing, the API is enabled, we can move forward to setting up the OAuth consent screen.**

## OAuth Consent Screen

1. Go to OAuth Consent Screen, under the API & Services menu.

![image](https://user-images.githubusercontent.com/38545800/156888747-05044e13-7c9f-4e87-b2fc-00f44a94b4ed.png)

2. Start filling out everything, don't make this public (unless you want too.)
3. Add your scopes, in this case /auth/cloud-translation
4. Assuming this is not part of a corporation, add yourself as a test user.
5. Save & go back to the dashboard

## Generating the OAuth2 Creds

1. Click Credentials in the API & Services Menu
2. Click Create Credentials --> OAuth Client ID --> Application-Type: Web Application


![image](https://user-images.githubusercontent.com/38545800/156889249-89e9209c-07f5-4d68-8aaf-5592ba391232.png)

3. Authorized Redirect URI
- Where are you storing your credentials to authenticate & authroize the OAuth flow? In this write up I am using Tines.
- For Tines you can find your callback uri in the OAuth2 when you are creating a OAuth2 credential. 

![image](https://user-images.githubusercontent.com/38545800/156889517-aabdcb02-505c-4d3c-98fb-d895336e8b26.png)

- You'd take the callback uri, and post it in the Authorized Redirect URI.

4. Save, Copy Credentials to your credential store.


## Hooking this into tines.io

1. Create new credential under "Your Team" (Or rename it)

![image](https://user-images.githubusercontent.com/38545800/156889721-26df1c86-b213-4c39-94a0-aa8e4256b0c5.png)

2. Fill everything out from google. Example below.

![image](https://user-images.githubusercontent.com/38545800/156889807-7a7cccfd-f27e-4fd3-9b5f-e10a2acae35b.png)

3. Save, and you'll be redirected to authorize the user. Authorize with your test user that you designated from above L41

Done!

Now  you can run a few tests!
