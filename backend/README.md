# Lucky Day Backend Coding Challenge

## Description 

The purpose of this assignment is to take an existing design from a relational database and migrate it to a NoSQL database design. You will also implement a web API that will perform a simple operation on this new database design.

## Goals

This challenge is designed to test your skills with:

* C# Fundamentals
* Building an API
* Object-Oriented Design
* Database Design
* Git

This challenge generally takes candidates no more than 6 hours to complete.

## Challenge
Bob has a new job as CTO of a social media startup company. To start off with, he creates a UsersProfile table with the following relational database schema:

**UserProfile Table**

| Column Name  | Data Type | Description |
| ------------- | ------------- |------------- |
| Id | INTEGER | Unique identifier |
| EMAIL | VARCHAR(100) | User's email address |
| FirstName | VARCHAR(100) | User's first name |
| LastName | VARCHAR(100) | User's last name |
| PhotoUrl | VARCHAR(100), NULL | User's photo url |
| PhoneNumber | VARCHAR(100), NULL | User's phone number |
| Region | VARCHAR(100), NULL | User's region area |
| SchoolName | VARCHAR(100), NULL | User's school name |
| SchoolStartYear | INTEGER, NULL | Year the user started school |
| SchoolEndYear | INTEGER, NULL | Year the user ended school |
| Industry | VARCHAR(100), NULL | User's industry |
| JobTitle | VARCHAR(100), NULL | User's job title |
| Company | VARCHAR(100), NULL | User's company |
| JobStartYear | INTEGER, NULL | Year the user started company |
| JobEndYear | INTEGER, NULL | Year the user ended company |
| Bio | VARCHAR(100), NULL | User's biography |
| Facebook | VARCHAR(100), NULL | User's Facebook url |
| Twitter | VARCHAR(100), NULL | User's Twitter handle |
| Blog | VARCHAR(100), NULL | User's blog url |

**Sample Data**

| Id | Email | FirstName | LastName | PhotoUrl | PhoneNumber | Region | SchoolName | SchoolStartYear | SchoolEndYear | Industry | JobTitle | Company | JobStartYear | JobEndYear | Bio | Facebook | Twitter | Blog | 
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| 1 | johnsmith@email.com | John | Smith | www.someimagehost.com/blahblahimage123.png | 3100000000 | Greater Los Angeles | University of California, Los Angeles | 2000 | 2004 | Software Professional | Software Developer | Fun Times, Inc | 2014 | Present | Experienced developer with a proven track record in .NET development | www.facebook.com/johnblahblah123 | @johnblahblah123 | www.johnblahblah123.net | 

Visually this application looks something like this:

![alt text](https://cf-s3-luckyday-test.luckydayapp.com/GitHub/jsmith.png)

All is well for Bob until his clients ask if he can incorporate additional fields for his user profiles. For instance, let's say there becomes a need to expand the user's education to include more than one school. Bob could dynamically add these new columns (i.e. SchoolName2, SchoolStartYear2, SchoolEndYear2, etc) on demand for his UsersProfile table, but that doesn't sound very scalable to him. As with many things, Bob took an interest in NoSQL years ago. He remembers the advantages that schema-less data can have for certain use cases, especially with varying metadata.

Armed with this information, Bob decides to re-architect his existing design.

## Requirements
1. Setup a public GitHub repository 'code-challenge' to commit and push your code.
2. Create a locally embedded NoSQL database, our recommendation is to use [LiteDB](http://www.litedb.org/) (it's free and easy to use!). If you do plan on using another third party provider, please be very detailed in your explanation for how to setup, run, and use this provider.
   - **IMPORTANT:** Spend some time to define your collection and schema design. How will your new design accommodate these new fields? Let's say we were to allow the user to store as many previous working experiences as they would like, would your design be able to scale?
3. In Visual Studio or whichever method you prefer, create a new .NET Framework or .NET Core project.
4. At a minimum create a web API with the following criteria below. Feel free to create more APIs though, if you feel you have something more ideal in mind. You can be as creative as you'd like with how you construct these APIs. For simplicity though, let's return a JSON response.
   1. Get a list of users given a particular region and industry.
5. Write a few local unit tests. At a minimum, please cover the basic success and failure scenarios.

**NOTE:** You do not need to implement any additional migration logic.

## Submission Guidelines

1. Setup a public GitHub repository 'code-challenge' to host the code.
2. Create a README file within the repository that contains the following:
   - Brief walkthrough of app design / choices made
   - Briefly explain your object oriented analysis and design
   - Provide a detailed explanation of your database design.
   - Local environment setup instructions to compile and run the app
   - Test suite setup/execution instructions (if applicable) 
3. Email links of your **public GitHub** repository and your name in subject line to [dev-challenge@luckydayapp.com](mailto:dev-challenge@luckydayapp.com)
