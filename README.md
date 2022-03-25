# White Label Exercise:
> School Of Whales\
> 03-24-2022\
> Eduardo Palomba

> This application was coded on Visual Studio Code using XAMPP, CodeIgniter 4, Compose, jQuery, Bootstrap and MySQL.
> Running on: http://localhost:8080/

**Attention:** As no database was mentioned on the test I chose MySql, so, please, **run de script you will find below to create de database and table**. Some adjust on CodeIgniter may be necesary on App > Config > Boot > Database **in case the hostname is <> localhost or password is not blank.**

> **Requisition: Create a CRUD using CodeIgniter**

1. The user should be able to input their:
      - first name,
      - last name, and
      - email.
2. The frontend should be build using jQuery.
3. Additionally, when a user submits the form:
      - an automated email should be sent to the admin email.

Delivery: You will submit your code via email using the link to your GitHub repository.

PS: Please be prepared to walk us through how you did the exercise and what tools you used.

> **Script to create a DATABASE on MySQL**
```
CREATE DATABASE testsow;

USE testsow;

CREATE TABLE IF NOT EXISTS `users` (
	  `id` int(11) NOT NULL PRIMARY KEY AUTO_INCREMENT,
	  `fname` varchar(40) NOT NULL,
	  `lname` varchar(40) NOT NULL,
	  `email` varchar(100) NOT NULL,
        `datatime` DATETIME
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```
