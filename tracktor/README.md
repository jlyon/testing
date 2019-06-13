# Send Email and SMS Alerts on Tracktor Status changes

[Install this library on Mesa](https://getmesa.com/install/shoppad/mesa-library/tracktor)

## Setup

### Email setup

There is no additional setup beyond customizing templates [#customizing-templates](see below)

### Twilio setup

1. Create a twilio account
2. Create a Twilio Project
3. Purchase a Twilio phone number (starting at USD $1/mo)
4. Copy your production `Account SID` from your Project's [Settings page](https://www.twilio.com/console/project/settings)
    and paste it into the `tracktor-twilio-sid` [Mesa Secrets](https://getmesa.com/go/secrets) field
5. Copy your production `Auth Token` from your Project's [Settings page](https://www.twilio.com/console/project/settings)
    and paste it into the `tracktor-twilio-token` [Mesa Secrets](https://getmesa.com/go/secrets) field
6. Customize your SMS templates [#customizing-templates](see below)

> Note: Twilio charges a per-SMS fee [starting at USD $0.01]()
    

## Customizing templates

To edit your email templates, go to the [Mesa Storage](https://getmesa.com/go/storage) tab.
 - For emails: edit the `tracktor-email-*.liquid` and `tracktor-email-subject-*` storage items
 - For SMS messages send via Twilio: edit the `tracktor-sms-*.liquid` storage items