# Dialogflow Fulfillment Library

The Dialogflow Fulfillment Library makes creating fulfillment for Dialogflow v1 and v2 agents for 8 chat and voice platforms on Node.js easy and simple. Cross-platform text, card, image, suggestion are supported for Actions on Google, Facebook, Slack, Telegram, Kik, Skype, Line, Viber and Dialogflow's simulator with custom payload support for all platforms.

![fulfillment library works with 8 platforms](https://raw.githubusercontent.com/dialogflow/dialogflow-fulfillment-nodejs/master/dialogflow-fulfillment-graphic.png "Dialogflow's fulfillment library works with 8 platforms")

Dialogflow fulfillment allows you to connect Dialogflow's natural language understanding and processing to your own systems, APIs, and databases. Using Fulfillment, you can surface commands and information from your services to your users through a natural conversational interface. For more about [Dialogflow Fulfillment](https://dialogflow.com/docs/fulfillment).

## When To Use This Library
This library is intended to be help building Node.js Dialogflow Fulfillment for multiple [integrations](https://dialogflow.com/docs/integrations/) (such as [Google Assistant](https://dialogflow.com/docs/integrations/google-assistant), [Slack](https://dialogflow.com/docs/integrations/slack)) or when you aren't sure what integration you plan on using.
+ If you are only interested in building Dialogflow fulfillment for the Google Assistant and don't plan on using other integrations, use the [Actions on Google NPM module](https://github.com/actions-on-google/actions-on-google-nodejs) ([actions-on-google](https://www.npmjs.com/package/actions-on-google)) which supports all Actions on Google features.

## Quick Start

1. [Sign-up/Log-in to Dialogflow](https://console.dialogflow.com/api-client/#/login)
2. Create a Dialogflow agent
3. Go to **Fulfillment >** Enable Dialogflow Inline Editor<sup> a.</sup> **> `package.json`** tab to add`"dialogflow-fulfillment": "^0.5.0"` to the `dependencies` object.
4. Select `Deploy`.

  <sup>a.</sup> Powered by Cloud Functions for Firebase

## Setup Instructions

 1. Import the appropriate class:

 ```javascript
const { WebhookClient } = require('dialogflow-fulfillment');
```

 2. Create an instance:

 ```javascript
const agent = new WebhookClient({request: request, response: response});
```

## References
* [Dialogflow Classes Reference](https://github.com/dialogflow/dialogflow-fulfillment-nodejs/tree/master/docs).
* [Dialogflow Documentation](https://docs.dialogflow.com).

## Issues and Questions
* For bugs, please add an issue on [Github](https://github.com/dialogflow/dialogflow-fulfillment-nodejs/issues).
* Questions? Try [StackOverflow](https://stackoverflow.com/questions/tagged/dialogflow).
* Current Limitations with Fulfillment:
    * No verification for platforms-specific incompatible response combinations (i.e. multiple cards are not supported in a single Actions on Google response).


## How To Make Contributions?
Please read and follow the steps in the CONTRIBUTING.md.

## License
See LICENSE.md.

## Terms
Your use of this sample is subject to, and by using or downloading the sample files you agree to comply with, the [Google APIs Terms of Service](https://developers.google.com/terms/).
