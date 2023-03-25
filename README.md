# Codechef-Task

In this task I was asked to create an employee/user database using sql tables. Using python connectivity one should be able to perform operations on it. 
I was also asked to make an encrypted login page before entering the database, however I was unable to figure that part out.

In terminal open sql whose password is set to user and:

create database company;

create table emp(
    -> empno int,
    -> name varchar(20),
    -> dept varchar(20),
    -> salary int);
Insert some values
for eg:
insert into emp values(2,'Aditi','HR','120382000');
