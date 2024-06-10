# Project-Katalon-API-Testing

# Objective 
This application focuses on how the API works by testing all API end points.

# App Usage Guide
### Requirements that must be inserted before running this application are :
- Using Groovy language based on Katalon Studio `version 9.5.0`
- Testing is done on the End-Point API provided by [Reqres](https://reqres.in/)
- Testing was carried out with the Google Chrome Website Browser `version 125.0.6422.142` (Official Build)

### Summary of Testing Results
In the implementation of testing, testing was carried out on 30 Test Cases with the results:
```
30 Passed
0 Failed
0 Not Executed
```
So the test result is 100% Passed

### Report
In testing, if you have to test one test case at a time, it will take a long time, so a **_Test Suite_** is made, so that you can run several test cases simultaneously, namely:
```
TS - GET RESOURCES
TS - GET USER BY ID 
TS - GET USER PER PAGE
TS - POST, PUT, AND DELETE USER
TS - REGISTER AND LOGIN
```
To make testing easier, a **_Test Suites Collection_** was created to run several Test Suites simultaneously, namely:
```
TS - TEST ALL
```
### End Point
The overall endpoints on Reqress tested in this project are :
#### GET User by Page
To get user data based on the page, which in Reqress provided 2 pages that will generate a response code `200 OK` and result user
```
https://reqres.in/api/users?page=1
https://reqres.in/api/users?page=2
```
#### GET User by ID
To get single user data based on ID, which in Reqress is provided with 12 IDs, which will produce a `200 OK` response code and the result of the user in question.
```
https://reqres.in/api/users/?id=1
https://reqres.in/api/users/?id=2
https://reqres.in/api/users/?id=3
https://reqres.in/api/users/?id=4
https://reqres.in/api/users/?id=5
https://reqres.in/api/users/?id=6
https://reqres.in/api/users/?id=7
https://reqres.in/api/users/?id=8
https://reqres.in/api/users/?id=9
https://reqres.in/api/users/?id=10
https://reqres.in/api/users/?id=11
https://reqres.in/api/users/?id=12
```
If the request id does not exist, it will generate a `404 NOT FOUND` response code and no result.
```
https://reqres.in/api/users/?id=99
```
#### POST User 
```
https://reqres.in/api/users
```
To add user data, by entering in the `HTTP BODY` with the `TEXT` and `JSON` attributes, which will produce a `201 CREATED` response code and the results of adding data:
```
{
    "name": "morpheus",
    "job": "leader"
}
```
#### PUT User 
To change user data based on its id such as changing data on id 7
```
https://reqres.in/api/users/7
```
Then by entering the `HTTP BODY` with the `TEXT` and `JSON` attributes, which will produce a `200 OK` response code and the results of data changes:
```
{
    "name": "morpheus",
    "job": "zion resident"
}
```
#### DELETE User

