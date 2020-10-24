## Add config.env file to config folder
- create new file in config folder and call it config.env
- add to the config.env
```
PORT = 3000
MONGO_URI = <Put your mongo database url here>
GOOGLE_CLIENT_ID = <Put your Google Client Id here>
GOOGLE_CLIENT_SECRET = <Put your Client Secret here>
```

## Creating the Google OAuth 2.0
- Go to google cloud console
- Create a project (Google Api Project)
- Go to API and Services
- Click + Enable and Services
- Find and click Google+ in the social Section
- Enable API / Manage
- Go to Credentials
- For OATH option, Click link 'Credentials in APIs & Services'
- Create Credentials and OAuth Client ID
- Choose Aplication type is Web Aplication
- In the Authorized redirect URIs, add callback Url (http://localhost:3000/auth/google/callback)
- (Add the callback url if you want to deploy it)
- and you will get Client ID and Client Secret
- add the Id and the secret to the config.env

## Start the app
```bash
# Install the dependencies
npm install

# Run in development
npm run dev

# Run in production
npm start
```