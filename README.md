# Test and deploy Twilio Serverless with GitHub Actions

This repo includes an example of automated testing and deployment of a [Twilio Serverless](https://www.twilio.com/docs/runtime) environment. 

## Instructions
1) Fork the repo.
2) Create the following repository secrets (_settings > secrets_):
  * `TWILIO_ACCOUNT_SID`: this is your Twilio account SID or your API key 
  * `TWILIO_AUTH_TOKEN`: this is your Twilio auth token or your API secret 
  * `TWILIO_SMS_API_KEY`: this is an API to send SMS (create one at https://www.twilio.com/console/sms/project/api-keys)
  * `TWILIO_SMS_SECRET_KEY`: this is the secret for the API key created above
  * `TWILIO_SMS_FROM`: Phone number in your Twilio account to send the SMS from
  * `TWILIO_SMS_TO`: Phone number to send the SMS to
3) To run the automated tests, create a Pull Request. GitHub Actions will automatically execute your tests.
4) To make a deployment, push a commit to the `main` branch. GitHub Actions will automatically deploy your Twilio Serverless environment.
