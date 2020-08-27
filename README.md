# Two Factor Authentication Starter App

This is an elementary  login authentication use case of two-factor authentication via SMS using Ruby SDK.

Steps for Installation : 
1. Copy `.env.example` and rename to `.env` and add the appropriate values. 
Example :

		EMAIL=tonystark@domain.com
		PASSWORD=domain@123
		CLIENT_ID=abcde123-12a1-1a23-1234-123a12345a1a
		CLIENT_SECRET=123abcde-a123-1234-abcd-ab12345c67d8
		BASE_URL=baseurl.domain.com
		PHONE_NUMBER=+16543219870
		DESTINATION_EMAIL=test@domain.com

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
