# SMS OTP Verification on Node.js

This sample project demonstrates how to use Twilio's SMS Messaging APIs 
to verify application user's phone numbers. 

## Configure the sample application

To run the application, you'll need to gather your Twilio account credentials and configure them
in a file named `.env`. To create this file from an example template, do the following in your
Terminal.

```bash
cp .env.example .env
```

Open `.env` in your favorite text editor and configure the following values. You will need all of these values before you continue.

| Config Value  | Description |
| :-------------  |:------------- |
`TWILIO_ACCOUNT_SID` | Your primary Twilio account identifier - find this [in the console here](https://www.twilio.com/console).
`TWILIO_API_KEY` | Used to authenticate - [generate one here](https://www.twilio.com/console/dev-tools/api-keys).
`TWILIO_API_SECRET` | Used to authenticate - [just like the above, you'll get one here](https://www.twilio.com/console/dev-tools/api-keys).
`SENDING_PHONE_NUMBER` | This phone number will be sending the SMS messages to the user. Either use a phone number you purchased through Twilio, or one you have verified with your account.
`CLIENT_SECRET` | It must match the server's config value. You can also disregard it from the code if needed, it's just a little bit of very basic security.

## Run the sample application

Now that the application is configured, we need to install our dependencies from npm.

```bash
npm install
```

Now we should be all set! Run the application using the `npm start` command.

```bash
npm start
```

Your application should now be running at [http://localhost:3000/](http://localhost:3000/). 

Check your config values, and then make sure everything looks good.

## License
MIT
