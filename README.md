# Getting Started with DocuSign Integrations at Hackathons

## Note: This repository has been deprecated and replaced by the DocuSign Quick Starts, please see below for the updated repositories:

[DocuSign Quick Start for Node: Sign a PDF via an embedded signing ceremony](https://github.com/docusign/qs-01-node-embed-signing-ceremony).

[DocuSign Quick Start for Node: Send an Envelope via email](https://github.com/docusign/qs-02-node-send-envelope).

[DocuSign Quick Start for Node: list the user's envelopes](https://github.com/docusign/qs-03-node-list-envelopes).

[DocuSign Quickstart API code examples with Curl](https://github.com/docusign/qs-curl).

[DocuSign Quick Start examples for Ruby and Ruby on Rails](https://github.com/docusign/qs-ruby).

[DocuSign Quick Start examples for Python](https://github.com/docusign/qs-python).

[DocuSign Quick Start examples for Java](https://github.com/docusign/qs-java).

[DocuSign Quick Start examples for C#](https://github.com/docusign/qs-csharp).

[DocuSign Quick Start examples for PHP](https://github.com/docusign/qs-php).

## Overview
In our Developer Center, we have complete [guides](https://developers.docusign.com/esign-rest-api/guides), [code examples](https://developers.docusign.com/esign-rest-api/code-examples), and [API reference](https://developers.docusign.com/esign-rest-api/reference). However, we know that at hackathons, you aren't looking for best practices. You just want to get your app working - fast! We've created this readme to get you running in minutes!

## Getting Started
### DocuSign Account Setup
Our eSignature API uses OAUTH which, for production environments, has a few steps to setup. For your hackathon project, you can bypass all of this with a temporary OUATH token (good for 8 hours) that is simple to generate. Here are the steps to take to get started:
1. Create a free [DocuSign developer account sandbox](https://go.docusign.com/o/sandbox/).
2. Locate your API Account ID by following these steps:
    1. Login to your sandbox account created above (if you are not already logged in).
    2. Note your **accountId** value as shown here:
    ![DocuSign Account Image](https://github.com/DocuSign-Hackathons/getting-started/blob/master/Images/DocuSignAccount.png "Account ID")
3. Navigate to [OAUTH Token Generator Page](https://developers.docusign.com/oauth-token-generator) and click **GET MY ACCESS TOKEN** and copy the token. You'll need this for your DocuSign API calls.
    1. Click on GET MY ACCESS TOKEN button
    2. Login with you Sandbox account
    3. Copy the token from the text box below "Access token granted to.." and paste it into each code example
    4. The token is typically valid for 8 hours. Don’t forget to come back and generate a fresh one!


### Node.js Examples
We have these Node.js examples in this repo that will get you running in minutes:
* **sendEnvelope.js** – Shows you how to send a DocuSign envelope via eMail
* **sendEnvelopeFromTemplate.js** – Shows you how to send a DocuSign envelope from a template stored in your DocuSign account
* **embeddedSigning.js** – Shows you how to embed (sign within your app) DocuSign functionality

Here's how you run each of the examples: 
1. Install the following npm dependencies:
    * npm i docusign-esign
    * npm i express
2. Open the desired sample Node.js example file from this repo and substitute the values you copied above into the **OAuthToken** and **accountId** variables.
3. If you are using the **sendEnvelopeFromTemplate** example, you'll need to upload a document to use as a template, then get the template ID, which you can find by logging into your DocuSign sandbox account clicking Templates in the top nav bar,  finding your template, and clicking the (i) icon, like this: ![TemplateID image](https://github.com/DocuSign-Hackathons/getting-started/blob/master/Images/TemplateID.png "Template ID")

## Additional Resources
* Real-time help: If you need any help from DocuSign engineers, contact us using the channel supported by the hackathon (devpost, Slack, etc.)
* [DocuSign Developer Center](https://developers.docusign.com)