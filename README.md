# CM business messaging API postman collection
Postman collection descriptions for CM.com's Business Messaging API. Full documentation available on [developers.cm.com/messaging/](https://developers.cm.com/messaging/).

## Requirements

You'll need a CM account with valid product token. To use channels other than SMS (WhatsApp, Viber, RCS, Apple Messages for Business, Facebook Messenger, Instagram, Google Business Messages, LINE, Telegram or Mobile Push), please visit [CM.com](https://www.cm.com/products/text/multi-channel-messaging/) and make sure your account is granted access to those channels.

This Postman Collection and Environment requires the installation of [Postman](https://www.getpostman.com/).


## Installing

1) Download `collection.json` and `environment.json` onto your local machine.
2) Open Postman, click on Import and select both files.
3) Once imported, a new API collection and a new environment will be created.
4) Select the **CM Business Messaging API** environment from the environment picker in the top-right of Postman.

## Environment variables

The collection uses the following variables, all of which are defined in `environment.json`. Fill in the values that apply to your situation:

| Variable        | Description                                                                                                |
|-----------------|------------------------------------------------------------------------------------------------------------|
| `ProductToken`  | Your CM product token, found in the [Channels app](https://www.cm.com/app/channels). Stored as a secret.   |
| `Sender`        | The sender of the message. Format depends on the channel (phone number, alphanumeric sender, Page ID, etc.).|
| `Recipient`     | The primary recipient identifier. Format depends on the channel (phone number, PSID, IGSID, etc.).         |
| `Recipient2`    | An optional second recipient, used by the multi-recipient SMS example.                                     |
| `Grouping`      | A custom grouping value, used by the SMS custom-grouping example.                                          |
| `WA_Namespace`  | The namespace for a WhatsApp template, provided by CM after the template is approved.                     |
| `AppKey`        | The Mobile Push channel account id, provided during Mobile Push onboarding.                               |
