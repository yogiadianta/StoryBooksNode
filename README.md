## Creating the Google OAuth 2.0
- Go to google cloud console
- Create a project (Google Api Project)
- Go to API and Services
- Click + Enable and Services
- Find and click Google+ in the social Section
- Enable API / Manage
- Go to Credentials
- For OATH option, Click link 'Credentials in APIs & Services'
- + Create Credentials and OAuth Client ID
- Choose Aplication type is Web Aplication
- In the Authorized redirect URIs, add callback Url (http://localhost:3000/auth/google/callback)
- (Add the callback url if you want to deploy it)
- and you will get Client ID and Client Secret
- add the Id and the secret to the config.env

## Using Passwordjs for Google OAuth 2.0
- Go to Passwordjs and choose passport-google-oauth20
