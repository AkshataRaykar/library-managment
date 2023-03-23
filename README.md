# library-managment
library mangement web application
library management is a software where the two user of the system admin and librarian manage the library. Admin can add librarian and librarian can add books veiw books issue the books and veiw issues books and also check the status of the book return. 

Technologies used : 
1. eclipse IDE
2.oracle database 

FRONT END: 
HTML
CSS
Javascript 

BACK END: 
oracle 10g database 

Steps to run project 
1.create three tables in oracle database manually using folowing statments. 
CREATE TABLE  "E_BOOK" 
   (	"CALLNO" VARCHAR2(4000), 
	"NAME" VARCHAR2(4000), 
	"AUTHOR" VARCHAR2(4000), 
	"PUBLISHER" VARCHAR2(4000), 
	"QUANTITY" NUMBER, 
	"ISSUED" NUMBER, 
	 CONSTRAINT "E_BOOK_PK" PRIMARY KEY ("CALLNO") ENABLE
   )
/
CREATE TABLE  "E_LIBRARIAN" 
   (	"ID" NUMBER , 
	"NAME" VARCHAR2(4000), 
	"PASSWORD" VARCHAR2(4000), 
	"EMAIL" VARCHAR2(4000), 
	"MOBILE" NUMBER, 
	 CONSTRAINT "E_LIBRARIAN_PK" PRIMARY KEY ("ID") ENABLE
   )
/


CREATE TABLE  "E_ISSUEBOOK" 
   (	"CALLNO" VARCHAR2(4000) NOT NULL ENABLE, 
	"STUDENTID" VARCHAR2(4000) NOT NULL ENABLE, 
	"STUDENTNAME" VARCHAR2(4000), 
	"STUDENTMOBILE" NUMBER, 
	"ISSUEDDATE" DATE, 
	"RETURNSTATUS" VARCHAR2(4000)
   )
/


2. create web application  project in eclipse IDE import the project 
3. create a server and run the application 


Project working : 

1.login as admin using the creintial : 
username : admin@gmail.com
password : admin123
2. add librarian click on veiw librarian then logout 
3. login as librarian add books issue books veiw issues books veiw the status of issues book delet the book.
