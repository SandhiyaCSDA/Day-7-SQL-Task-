# Day-7-SQL-Task-
Day 7 SQL Task
# DELETE
create table students(
Serial_no int,
Name varchar(50),
Age int,
Department Varchar(50),
Phone_Number varchar(20)
);
alter table students change serial_no Student_ID varchar(10);
alter table students modify phone_number varchar(20);
select * from students;
insert into students(Student_id,Name,Age,Department,Phone_Number)
values
('24UCSD001','AUGUSTIN',19,'COMPUTER SCIENCE','6358749612'),
('24UBCO002','LATHA',20,'BCOM','8596321474'),
('24UCSD004','DEEPIKA',19,'COMPUTER SCIENCE','8965741236'),
('24UBAA004','ARUN',18,'BBA','9658741236'),
('24UCSD006','ARSHATH',19,'COMPUTER SCIENCE','6987456321'),
('24UBCO005','SHRUTHI',20,'BCOM','9685741232'),
('24UCSD008','ABINITHI',20,'COMPUTER SCIENCE','8958741236'),
('24UBAA010','KARTHI',18,'BBA','6358741236'),
('24UCSD020','RAGU',19,'COMPUTER SCIENCE','6987456111'),
('24UBCO021','SHRUTHI',20,'BCOM','9685741222');
select * from students;
delete from students 
where student_id = '24UBCO005';
select * from students;
# Truncate
use RK_HOSPITAL;
create table paitent(
Serial_No int,
Name varchar(100),
Age int,
Date_Of_Birth date,
Gender varchar(1),
Phone_Number varchar(20),
Place varchar(50),
Doc_Fee Decimal(11,3),
Weight Float,
Temperature Float,
Causes Varchar(50)
)
select * from paitent;
truncate table paitent;
# Drop
use students;
alter table students add email_id varchar(50);
select * from students;
alter table students drop column email_id;
select * from students;
