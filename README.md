# Project-Katalon-API-Testing

# Objective 
This application focuses on how the API works by testing all API end points.

# App Usage Guide
### Requirements that must be inserted before running this application are :
- Using Groovy language based on Katalon Studio version 9.5.0
- Testing is done on the End-Point API provided by [Reqres](https://reqres.in/)
- Testing was carried out with the Google Chrome Website Browser version 125.0.6422.142 (Official Build)

### Summary of Testing Results
In the implementation of testing, testing was carried out on 30 Test Cases with the results:
```
30 Passed
0 Failed
0 Not Executed
```
So the test result is 100% Passed

### Report
In testing, if you have to test one test case at a time, it will take a long time, so a **Test Suite** is made so that you can run several test cases simultaneously, namely:
```
TS - GET RESOURCES
TS - GET USER BY ID 
TS - GET USER PER PAGE
TS - POST, PUT, AND DELETE USER
TS - REGISTER AND LOGIN
```
To make testing easier, a **Test Suites Collection** was created to run several Test Suites simultaneously, namely:
```
TS - TEST ALL
```
