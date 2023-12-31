# Epic & Feature Rightsizing for Jira & Azure DevOps

### What is this report? 
This will detail, based on your historical completed Epics and/or Features, what was the size of these items (in terms of child item count). It will also detail what the size is (in terms of child item count) of your current ‘in progress’ or ‘planned’ Epics and/or Features.

### Why would you use it? 
Aiming for consistency around the size of Epics and/or Features improves our ability to be more predictable around forecasting delivery and also means we don’t have work remaining open indefinitely. 

### When would you use it?
Use this when trying to understand what the ‘right size’ is for your Epics and/or Features is. Similarly you might want to use this when planning work for a quarter/semester. You may also want to use it when you have a hunch about an ever increasing scope to a piece of work.

### Prerequisites
* [Make sure you have the latest version of Power BI Desktop](https://aka.ms/pbiSingleInstaller)
* Download the appropriate template file:
  - [Jira version](https://github.com/nbrown02/EpicFeatureRightsizing/raw/main/Rightsizing%20(Jira).pbit)
  - [Azure DevOps version](https://github.com/nbrown02/EpicFeatureRightsizing/raw/main/Rightsizing%20(Azure%20DevOps).pbit)
* If you are setting this up for Jira then [follow these steps](https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/) to setup a Jira API token and note it down (e.g. copy/paste into Notepad)
* If you are setting this up for Azure DevOps then [follow these steps](https://learn.microsoft.com/en-us/azure/devops/organizations/accounts/use-personal-access-tokens-to-authenticate?view=azure-devops&tabs=Windows#create-a-pat) to setup a Personal Access Token (PAT) with full access and note it down (e.g. copy/paste into Notepad)
* Then you're good to get started!

### Connectivity & Data Load
* Open the relevant .pbit file in Power BI Desktop
* For Jira:
  - Add your Jira URL
  - Add your Jira Project Key
* For Azure DevOps:
  - Select http/https (only choose http if your Azure DevOps Server is HTTP)
  - Add the Analytics / Azure DevOps Server URL - for Azure DevOps services enter 'analytics.dev.azure.com' / for Azure DevOps Server enter your server details
  - Add your Organization / Project / Team Name

* It should then look something like this (for Jira):
![image](https://github.com/nbrown02/EpicFeatureRightsizing/assets/29369962/60988366-f440-46e5-9153-2967712ebca1)

* Or this (for Azure DevOps):
![image](https://github.com/nbrown02/EpicFeatureRightsizing/assets/29369962/8641b0eb-e0bc-4379-9080-4aba4ffae9a6)

* Hit 'Load' 
* You will be prompted for a login
* For Jira, choose Basic and enter:
  - Your email associated with your Jira account for your username
  - Your API token you created in the Prerequisities

![alt text](https://raw.githubusercontent.com/nbrown02/FlowViz-Jira/main/Screenshots/Login2.png)

* For Azure DevOps, choose Basic and enter:
  - Your Personal Access Token (PAT) to login, entering it in the password field (user can be left as blank - make sure it has 'Read' access to Analytics)

![alt text](https://docs.microsoft.com/en-us/azure/devops/report/powerbi/media/authentication-7.png?view=azure-devops)

* Then hit 'Connect' and wait for the data and charts to load!

### Screenshots

Jira:
![alt text](https://raw.githubusercontent.com/nbrown02/EpicFeatureRightsizing/main/Jira1.png)

Azure DevOps (as ADO has a three-level hierarchy the view is slightly different):
![alt text](https://raw.githubusercontent.com/nbrown02/EpicFeatureRightsizing/main/ADO1.png)

![alt text](https://raw.githubusercontent.com/nbrown02/EpicFeatureRightsizing/main/ADO2.png)

### Using the report
Based on the selected date range you can see the right size (85th percentile) for Epics/Features in terms of their child item count. You may want to look at those 'open' Epics/Features and those items that have been ‘red flagged’ as being bigger than this and think about reducing the scope of this.

Similarly, we might want to look at the yellow warning next to our Epic/Feature as this now is nearly bigger than 85% of those Epics/Features previously. Here you might want to be having conversations around scope and the rate at which this is growing and the potential risks this may be bringing about in elongating the feedback loop to what it is we are working on.

### Feedback
This template is built and maintained by [Nicolas Brown](https://www.nicolasbrown.co.uk/) use [the issues section]((https://github.com/nbrown02/EpicFeatureMonteCarlo/issues)) for any bugs you find and [the discussion section](https://github.com/nbrown02/EpicFeatureMonteCarlo/discussions) for any question, ideas and/or feature requests.
