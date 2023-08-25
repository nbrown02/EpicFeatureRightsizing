# Epic & Feature Rightsizing Template

## What is this report? 
This will detail, based on your historical completed Epics and/or Features, what was the size of these items (in terms of child item count). It will also detail what the size is (in terms of child item count) of your current ‘in progress’ or ‘planned’ Epics and/or Features.

## Why would you use it? 
Aiming for consistency around the size of Epics and/or Features improves our ability to be more predictable around forecasting delivery and also means we don’t have work remaining open indefinitely. 

## When would you use it?
Use this when trying to understand what the ‘right size’ is for your Epics and/or Features is. Similarly you might want to use this when planning work for a quarter/semester. You may also want to use it when you have a hunch about an ever increasing scope to a piece of work.

## Steps to load the information
Download the template using this link
Open the template in Power BI Desktop
Enter your Organization / Project / Team Name details in the fields provided:
Hit load
Note: you may be asked for a login - follow these steps if it’s your first time
Then your data is loaded

## Using the report
There are a few different ways you can use the report. For example, you might want to focus on the count of Features that are under an Epic, if so you’d use a view similar to this:

IMAGE

Based on the past 18 weeks we can see that the right size (85% of the time) for our Epics was to have 11 Features or less underneath them. We therefore might want to look at those items that have been ‘red flagged’ as being bigger than this and think about reducing the scope of this. Similarly, we might want to look at the yellow warning next to our Epic which already has 11 child Features as this now is nearly bigger than 85% of the work previously. Here you might want to be having conversations around scope and the rate at which this is growing and the potential risks this may be bringing about in elongating the feedback loop to what it is we are working on. The same logic can be applied when looking at Epic size in terms of child items at Feature AND Story level (it also cross filters to show where the bigger sizing may be occurring): 

IMAGE

This is helpful when your Feature count is ‘right-sized’ but at story level you might want to just check there aren’t too many items. You can also use this to look at the count of items at Story level (including custom items) within a Feature. The title column in every table is a hyperlink that will take you to that respective item in Azure DevOps.
It’s worth noting that there is no universal right-size - just consider this as a tool you can use to keep track on the size of items and potentially intervene if needed.
