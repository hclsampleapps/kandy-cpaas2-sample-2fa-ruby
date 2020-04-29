# Two Factor Authentication Starter App

This is an elementary  login authentication use case of two-factor authentication via SMS using Ruby SDK.

Steps for Installation : 
1. Copy `.env.example` and rename to `.env` and add the appropriate values. 
Example :

EMAIL=test@gmail.com
PASSWORD=Test@123
CLIENT_ID=faaaf096-73a1-4f48-9814-674a30562b0r
CLIENT_SECRET=4d821aba-c758-4294-b57a-cb5e416c32e9
BASE_URL=https://oauth-cpaas.att.com
PHONE_NUMBER=+12015645539
DESTINATION_EMAIL=test@gmail.com

2. To install dependencies, run:
bundle install

3. To start the server, run:
bundle exec rackup -p 6001

ENV KEY           | Description
----------------- | -------------
CLIENT_ID         | Private project key
CLIENT_SECRET     | Private project secret
BASE_URL          | URL of the CPaaS server to use
PHONE_NUMBER      | Phone number that would receive the verification code
EMAIL             | Email used in the login screen of the application
PASSWORD          | Password to be entered against the EMAIL provided in the login screen 
DESTINATION_EMAIL | Email that would receive the verification code