# Getting Started with DocuSign Integrations at Hackathons


## Overview
In our Developer Center, we have complete [guides](https://developers.docusign.com/esign-rest-api/guides), [code examples](https://developers.docusign.com/esign-rest-api/code-examples), [Quickstart guides](https://developers.docusign.com/docs/esign-rest-api/quickstart/overview/), and [API reference](https://developers.docusign.com/esign-rest-api/reference). However, we know that at hackathons, you aren't looking for best practices. You just want to get your app working, fast! We've created this readme to get you running in minutes!

## Getting Started
### DocuSign Account Setup
Our eSignature API uses OAUTH which, for production environments, has a few steps to set up. For your hackathon project, you can bypass all of this with a temporary OUATH token (good for 8 hours) that is simple to generate. Here's how to get started:
1. Create a free [DocuSign developer account](https://go.docusign.com/o/sandbox/).
2. Locate your API Account ID by following these steps:
    1. Log in to your developer account created above (if you are not already logged in).
    2. Note your **accountId** value as shown here:
    ![DocuSign Account Image](https://github.com/docusign/Hackathons-getting-started/blob/main/Images/DocuSignAccount.png "Account ID")
3. Navigate to the [OAUTH Token Generator Page](https://developers.docusign.com/token-generator/), click **LOG IN**, and then copy the token. You'll need this for your DocuSign API calls.
    1. Click the LOG IN button
    2. Log in with your Sandbox account
    3. Copy the token from the text box below "Access token granted to" and paste it into each code example
    4. The token is typically valid for 8 hours. Don’t forget to come back and generate a fresh one!


### Node.js examples
We have the following Node.js examples in this repo that will get you running in minutes:
* **sendEnvelope.js**: Shows you how to send a DocuSign envelope via email
* **sendEnvelopeFromTemplate.js**: Shows you how to send a DocuSign envelope from a template stored in your DocuSign account
* **embeddedSigning.js**: Shows you how to embed (sign within your app) DocuSign functionality

Here's how you run each of the examples: 
1. Install the following npm dependencies:
    * npm i docusign-esign
    * npm i express
2. Open the desired sample Node.js example file from this repo and substitute the values you copied above into the **OAuthToken** and **accountId** variables.
3. If you are using the **sendEnvelopeFromTemplate** example, you'll need to upload a document to use as a template, then get the template ID, which you can find by logging into your DocuSign developer account, clicking Templates in the top nav bar, finding your template, and clicking the (i) icon, like this:  
    ![TemplateID image](https://github.com/docusign/Hackathons-getting-started/blob/main/Images/TemplateID.png "Template ID")

## Additional resources
* Real-time help: If you need any help from DocuSign engineers, contact us using the channel supported by the hackathon (devpost, Slack, etc.)
* [DocuSign Developer Center](https://developers.docusign.com)