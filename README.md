# Assign-number-on-submit
Provides a basic JavaScript to assign number (normally primary key) to record on submit from FormBridge

## Motivation
It is known that [monthly-basis or daily-basis numbering capability](https://guide.kintoneapp.com/formbridge/automatic-numbering/) is provided.
However, other numbering such as annual numbering, and numbering based on fiscal year is sometimes required.
Therefore, let's develop custom numbering (or more precisely numbering based on fiscal year) by using JavaScript.

## Idea
FormBridge has a capability to add a record to kintone, but does not have any knowledge of other records currently processing.
Here, kViewer can provide External API, so it could be able to obtain latest number (or largest number assigned) by using kViewer External API.
Then, you can get new number to be assigned by incrementing the latest number obtained.

## Prerequisite
- FormBridge with premium license or higher
- kViewer External API
