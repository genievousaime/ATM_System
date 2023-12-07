# ATM_System
ATM Management System Project in Java. It’s a GUI-based project used with the Swing module to manage ATM transactions of a bank.

As partial fulfilment of SOFTWARE ENGINEERING GROUP PROJECT 4 under supervision of Dr. Balaji A.
Team Members:  
Urvi Kashyap - 21BCE10504  
Ruchika Roy - 21BCE10120  
Sanay Singh Rajawat - 21BCE10781  
Nayan Paliwal - 21BCE10163  
Manav Tirumal - 21BCE11528  
Priyansh Mishra - 21BCE10136  

## Setting up the Environment
Make sure JDK is present in your system. It can be installed using the IDE you are using.

The first step is to create a project in the name you wish. Create a package named “atm“. We are creating java classes in this package.

To connect the project to the database, follow the steps:

Make sure MySQL is installed on your system.
Download the MySQL connector.
Open the properties of the project from the dropdown list which appears on right-click on the project. Navigate to the libraries tab and click on the classpath. Select “Add External JARs…”. Select the connector sql file downloaded. This step will differ on IDE being used.

## MySQL Setup for ATM System
### 1. Creating the database
```
--CREATING THE DATABASE
CREATE DATABASE atm;
```
### 2. Selecting the database
```
--SELECTING THE DATABASE
USE atm;
```
### 3. Create a users table
```
--CREATE USERS TABLE
CREATE TABLE users(id int primary key auto_increment, card varchar(16), pin varchar(4), uname varchar(25), bal int);
```
### 4. Create a transaction table
```
--CREATE TRANSACTION TABLE
CREATE TABLE transactions(transid int primary key auto_increment, id int, amount int, stat varchar(3), bal int);
```
### 5. Create an admin user
```
--CREATING AN ADMIN USER
INSERT INTO users VALUES(1, "admin", "1234", "admin", 0);
```

## Login Page

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/f9f4451d-403e-4676-982f-c57bd0c050de"> 

Enter the card number in the text field and continue to enter the pin. Admin login in the bottom right helps you to log in as admin.  

## Pin Checking Page  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/91bca36c-a57c-4f84-9238-3401c2f034c0">  

Type the pin to your card, for admin enter “1234” as the pin. It will take you to your respective pages.  

## Admin home page  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/7f0dc065-9b6d-46f6-9c68-3176de318af6">  

Add user button directs you to a page where you can add users with their current balance.  


The exit button closes the application.  

## Module to add users  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/73455915-4ea5-4852-b6a3-0eebfb2f51a3">  

Enter name and balance to add the user into the system. The part of admin ends here.  

## Success Page  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/e5927090-bc90-4abc-a6eb-f4ae8ce9692a">  

Here we have a page labeled “TRANSACTION SUCCESSFUL“. There is also another method executed in this class if adding users is done. 

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/438e4ca6-c3cc-4789-8936-674aef040624">  

## Failed Transaction Page  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/fe87ec99-4fcb-4734-983c-44ed02b9e920"> 

## Home Page for Users  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/d521996f-9a5b-4e13-afef-9ebb3b04a0a3">  

## Quick Cash Window  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/ac1951f5-a3e7-44e4-a93d-2292aaef6d24">  

Here many amounts are fed by default. By Selecting any one of them, that amount will be remitted from the account balance.  

## Other Operations  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/9e6bdcda-e60e-48db-ad2c-b30b118bf5dc">  

All data for the deposit, withdrawal, changing pin, etc… are fed here. Enter the data and press SUBMIT to continue the transaction.  

  
## Bank statements  

<img width="403" alt="image" src="https://github.com/genievousaime/ATM_System/assets/91481594/64d75eba-86b4-4cd0-b22c-31e562adcef7">  

As we can see above, The deposit and withdrawal amounts are stated with the current balance. The latest transactions are represented first. 









