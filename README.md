# Medusa Twilio Message Plugin

The Twilio Message Plugin offers a way to interact with the Message API from Medusa events.

![cover image with stars and colored shading in the background as well as foreground text MEDUSA HACKATHON SUBMISSION Twilio Message Plugin](https://user-images.githubusercontent.com/116348315/197195527-6768341b-f51f-4f17-bdce-aa36bee253ed.png)

## Installation
 - install & setup medusajs/medusa
 - clone this repo
 - link with your package manager, [see the docs](https://docs.medusajs.com/advanced/backend/plugins/create/#test-your-plugin)
 - register/login at twilo, get your account sid & auth token
 - verify your phone number to send message to yourself
 - edit config (see below)
 - run & have fun

## Config
Follwowing changes must be made your medusa-config.js:
```js
{
	resolve: `medusa-plugin-twilio-message`,
	options: {
		ORDER_DISCOUNT_THRESHOLD: `<double>`, //threshold from 0.0 to 1.0
		TWILIO_ACCOUNT_SID: `ACXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX`, // Find your Account SID at twilio.com/console
		TWILIO_AUTH_TOKEN: `bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb` // Find your Auth Token at twilio.com/console
		SENDER_N_RECIPIENT: `+1999999999` //destination phone number in E.164 format
	}
}
```
