Poultry Farm Management System (PFMS)
Overview
The Poultry Farm Management System (PFMS) is a web-based application designed to help manage the daily operations of a poultry farm. It includes features for inventory management, order processing, and user administration.

Installation Guide
Prerequisites
XAMPP, WAMP, or LAMP stack installed
PHPMyAdmin access
Steps to Run the Project
Download the zip file

Download the project zip file from the provided source.
Extract the file

Extract the contents of the zip file to a local directory.
Copy the farm folder

Locate the extracted farm folder and copy it.
Paste inside the root directory

For XAMPP, paste the farm folder inside xampp/htdocs.
For WAMP, paste the farm folder inside wamp/www.
For LAMP, paste the farm folder inside var/www/html.
Open PHPMyAdmin

Open a web browser and go to http://localhost/phpmyadmin.
Create a database

Create a new database named poultry.
Import the SQL file

In PHPMyAdmin, select the poultry database.
Go to the Import tab and import the poultry.sql file located in the SQL file folder within the zip package.
Run the script

Open a web browser and navigate to http://localhost/farm.
Admin Credentials
Username: admin
Password: 1234
Database Structure
Tables
permissions
id (int, Primary Key)
permission (varchar)
createuser (varchar)
deleteuser (varchar)
createbid (varchar)
updatebid (varchar)
store_out
id (int, Primary Key)
date (date)
item (varchar)
quantity (varchar)
itemsoutvalue (int)
store_stock
id (int, Primary Key)
date (date)
item (varchar)
quantity (varchar)
rate (varchar)
total (varchar)
quantity_remaining (varchar)
itemvalue (int)
status (varchar)
tbladmin
ID (int, Primary Key)
Staffid (int)
AdminName (varchar)
UserName (varchar)
FirstName (varchar)
LastName (varchar)
MobileNumber (bigint)
Email (varchar)
Status (int)
Photo (varchar)
Password (varchar)
AdminRegdate (timestamp)
tblcategory
id (int, Primary Key)
CategoryName (varchar)
CategoryCode (varchar)
PostingDate (timestamp)
tblcompany
id (int, Primary Key)
regno (varchar)
companyname (varchar)
companyemail (varchar)
country (varchar)
companyphone (int)
companyaddress (varchar)
companylogo (varchar)
status (varchar)
developer (varchar)
creationdate (timestamp)
tblitems
id (int, Primary Key)
item (varchar)
description (varchar)
Creationdate (timestamp)
tblorders
id (int, Primary Key)
ProductId (int)
Quantity (int)
InvoiceNumber (int)
CustomerName (varchar)
CustomerContactNo (bigint)
PaymentMode (varchar)
InvoiceGenDate (date)
tblproducts
id (int, Primary Key)
CategoryName (varchar)
ProductName (varchar)
ProductImage (varchar)
ProductPrice (decimal)
PostingDate (timestamp)
UpdationDate (timestamp)
Auto-increment Settings
permissions -> id (auto-increment)
store_out -> id (auto-increment)
store_stock -> id (auto-increment)
tbladmin -> ID (auto-increment)
tblcategory -> id (auto-increment)
tblcompany -> id (auto-increment)
tblitems -> id (auto-increment)
tblorders -> id (auto-increment)
tblproducts -> id (auto-increment)
