# 📚 Library Management System -Java

A Library Management System made using the concepts of Object Oriented Analysis and Design. Minimal Code is written in the GUI and the entities are decoupled as well. The interface is console based. This project was designed during the course "Object Oriented Analysis and Design CS309".  

## Actors:
The actors include the following: 
* Librarian
* Checkout Clerk
* Borrower
* Administrator

## Use Cases:
After determining the actors, the second step in use case analysis is to determine the tasks that each actor will need to do with the system. Each task is called a use case because it represents one particular way the system will be used.

**In other words, only those use cases are listed that actors will need to do when they are using the system to solve the customer’s problem.** 

### Borrower:
* ❏ Search for items by title.
* ❏ ... by author.
* ❏ ... by subject.
* ❏ Place a book on hold if it is issued to somebody else.
* ❏ Check  the  borrower’s  personal  information  and  list  of  books  currently
borrowed.

### Checkout Clerk:
* ❏ All the Borrower use cases, plus
* ❏ Check out an item for a borrower.
* ❏ Check in an item that has been returned.
* ❏ Renew an item.
* ❏ Record that a fine has been paid.
* ❏ Add a new borrower.
* ❏ Update a borrower’s personal information (address, telephone number etc.).

### Librarian:
* ❏ All of the Borrower and Checkout Clerk use cases, plus
* ❏ Add a new item to the collection.
* ❏ Delete an item from the collection.
* ❏ Change the information the system has recorded about an item.

### Administrator:
* ❏ Add Clerk.
* ❏ Add Librarian.
* ❏ View Issued Books History.
* ❏ View All Books in Library.


## How to Run
1- Install these:
 * [Java SE Development Kit 8 (JDK 8)](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
 * After installing JDK 8, install [NetBeans IDE](https://netbeans.org/downloads/)

2- Open NetBeans IDE. Click on File -> Open Project and browse to the downloaded folder named "Project" and select it. It will load the NetBeans project.

3- Now everything is setup except the XAAMP MySql database for NetBeans. So, follow these steps to setup the database:

**Step 1:** First download the XAAMP server extension from [XAAMP](https://www.apachefriends.org/download.html) then open the live apache server and click 'start' on MySql
data server on port 3306.
   
**Step 2:** After that create a database named library_ms that will show up on phpmyadmin tab. To get phpmyadmin tab click on [phpmyadmin](http://127.0.0.1/phpmyadmin/).
   
**Step 3:** Provide the following database crendentials in the next popup and click Next.
  ```
  Host: localhost
  Port: 3306
  Database: library_ms
  User Name: 
  Password: 
  ````
**Step 4:** Now just click Next for the rest of the windows. After all this the database connection is made. Make sure that you connect with the database before running the project by right clicking on the connection and selecting connect. Now you are ready to run the project!

**Step 5:** Now to create the user table, issue_book table, student table etc, we have to write some sql querries in the database.
1- create database library_ms;
2- create table users(id int PRIMARY KEY AUTO_INCREMENT NOT null, name varchar(50), password varchar(50), email varchar(100), contact varchar(20));
3- create table books_details(book_id int PRIMARY key not null, book_name varchar(100), author_name varchar(200), quantity int);
4- create table student_details(student_id int PRIMARY KEY NOT null, student_name varchar(30), course_name varchar(50), branch varchar(50));
5- create table issue_book_details(id int PRIMARY KEY NOT null AUTO_INCREMENT, book_id int, book_name varchar(150), student_id int, student_name varchar(50), issue_date date,      due_date date, status varchar(20));
6- select book_name, count(*) as count from issue_book_details group by book_id;

## 🤝 Consulting
Stuck with some problem? Need help in solution development, guidance, training or capacity building? I am a Full Stack Developer with technical and leadership experience in a diverse range of technologies and domains. Let me know what problem you are facing at <b>soumya261412@gmail.com</b>.

## 👨‍💻 Technical Skills & Expertise

- Development of Web Applications, Mobile Applications, and Desktop Applications
<hr>

## Authors 👋

You can get in touch with us on our LinkedIn Profiles:

#### Soumya Ranjan Rout

[![LinkedIn Link](https://img.shields.io/badge/Connect-harismuneer-blue.svg?logo=linkedin&longCache=true&style=social&label=Follow)](https://www.linkedin.com/in/harismuneer)

You can also follow my GitHub Profile to stay updated about my latest projects: [![GitHub Follow](https://img.shields.io/badge/Connect-harismuneer-blue.svg?logo=Github&longCache=true&style=social&label=Follow)](https://github.com/harismuneer)

#### Maham Amjad

[![LinkedIn Link](https://img.shields.io/badge/Connect-maham--amjad-blue.svg?logo=linkedin&longCache=true&style=social&label=Connect)](https://www.linkedin.com/in/maham-amjad-40796b177/)

You can also follow my GitHub Profile to stay updated about my latest projects: [![GitHub Follow](https://img.shields.io/badge/Connect-maham--amjad-blue.svg?logo=Github&longCache=true&style=social&label=Follow)](https://github.com/MahamAmjad)

If you liked the repo then kindly support it by giving it a star ⭐ and share in your circles so more people can benefit from the effort.

## Contributions Welcome
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](#)

If you find any bug in the code or have any improvements in mind then feel free to generate a pull request.

## Issues
[![GitHub Issues](https://img.shields.io/github/issues/harismuneer/Library-Management-System-JAVA.svg?style=flat&label=Issues&maxAge=2592000)](https://www.github.com/harismuneer/Library-Management-System-JAVA/issues)

If you face any issue, you can create a new issue in the Issues Tab and I will be glad to help you out.
