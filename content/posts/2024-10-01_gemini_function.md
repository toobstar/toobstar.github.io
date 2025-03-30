+++
title = 'Fixing a missing feature of Google Workspace to improve the Gemini AI Assistant'
date = 2024-10-13T09:24:56+11:00
draft = true
tags = ['Collaboration', 'CIO', 'Integration', 'Productivity']
revision = 1
+++

![Improving Gemini AI](https://toobstar.github.io/images/caveman_computer.jpg)

## Implementing a missing (but obvious) feature of Google Gemini AI assistant.  

As compelling at Google's Gemini features are, and the fact they are sprinkled across the Google Product suite (including Sheets) it seems like a massive oversight to not allow users to make a direct function call from a spreadsheet cell to Gemini.  By having this in place you can do bulk updates that auto-refresh from Gemini and can directly interact with existing spreadsheet data in an extremely useful way. 


![Gemini Prompt in Google Sheets](https://toobstar.github.io/images/sheets_gemini_recording.mov)
![Gemini Prompt in Google Sheets](https://toobstar.github.io/images/sheets_gemini_prompt.gif)



[This approach](https://developers.google.com/workspace/add-ons/overview) allows you to do that via:

1) [A Google Workspace Apps Script](https://github.com/toobstar/google-workspace-apps-scripts/blob/main/google-sheets-gemini-function.js)
2) That has been configured to run in Google Cloud Platform (GCP)
3) And has a Google Workspace Marketplace listing to enable it to be installed as an extension

Before setting up the code in the script you need to [create an API key in the Google AI Studio](https://aistudio.google.com/app/apikey).  The script itself simply facilitates the google-sheet [custom function logic](https://sheetbest.com/blog/deploying-google-sheets-custom-functions/) making a request into the API.  

After creating a project at script.google.com and copying the [code](https://github.com/toobstar/google-workspace-apps-scripts/blob/main/google-sheets-gemini-function.js) in you then need to enable the GCP link after also creating the GCP project:

![Getting Clarity](https://toobstar.github.io/images/sheets_gemini_gcp.jpg)

You also need to deploy the application and note the version you are at which will go in the marketplace listing configuration. 

From the GCP project page you can then create an app marketplace listing which will eventually appear [here](https://developers.google.com/workspace/marketplace/manage-app-listing):

To update the configuration or details of your app listing, follow these steps:

1) In the Google Cloud console, go to Menu > APIs & Services > Google Workspace Marketplace SDK > App Configuration.

2) On the App Configuration tab, update your configuration details, and then click Save.

3) On the Store Listing tab, make your changes, and then click Publish.

After all this the application will be available to install in the [Google Workpace marketplace](https://workspace.google.com/marketplace).  This process should of course only be used for internal users in a controlled environment to avoid the API usage being uncontrolled. The application can actually be pushed to all users in an enterprise environment from the Google Worskpace admin console. 

