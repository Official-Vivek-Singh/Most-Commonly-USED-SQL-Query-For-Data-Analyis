# Most-Commonly-USED-SQL-Query-For-Data-Analyis

# Create a Table

CREATE TABLE COMPUTER 
(
		COMPID Int PRIMARY KEY,
		BRAND VARCHAR(50),
		COMPMODEL VARCHAR(50),
		MANUFACTUREDATE DATE
);

-- Above With the Help of DDL Commnad, We created a Table Using Create Statement

# Insert Data into Table

INSERT INTO COMPUTER VALUES(1001,'Lenovo','T480','2019-06-12');
INSERT INTO COMPUTER VALUES(1002,'Lenovo','T490','2020-08-24');
INSERT INTO COMPUTER VALUES(1003,'SONY','SQ112','2019-12-01');
INSERT INTO COMPUTER VALUES(1004,'SONY','SX1001','2020-12-21');

-- Above We interted the Data into Computer Table
- Using Insert Statement of DML(Data Manupulation Language

- # Create Employee Table

CREATE TABLE EMPLOYEE_Comp
(
		EMPID int PRIMARY KEY,
		FIRSTNAME VARCHAR(50),
		LASTNAME VARCHAR(50),
		SALARY double,
		EMAILID VARCHAR(50),
		MANAGERID int,
		DATEOFJOINING DATE,
		DEPT VARCHAR(10),
		COMPID int ,
		CONSTRAINT FK_COMPID FOREIGN KEY (COMPID) REFERENCES COMPUTER(COMPID)
);

# Insert Data Into Table

INSERT INTO EMPLOYEE_Comp VALUES(1,'NANDA','KUMAR',50000,'NANDA@GMAIL.COM',NULL,'2012-06-15','IT',1001);
INSERT INTO EMPLOYEE_Comp VALUES(2,'BIPLAB','PARIDA',30000,'BPARIDA@YAHOO.COM',1,'2015-12-21','IT',1001);
INSERT INTO EMPLOYEE_Comp VALUES(3,'DISHA','PATEL',50000,'DISHAP@GMAIL.COM',NULL,'2013-08-21','HR',NULL);
INSERT INTO EMPLOYEE_Comp VALUES(4,'SIBA','PRASAD',90000,'SIBA@GMAIL.COM',3,'2020-06-01','HR',1002);
INSERT INTO EMPLOYEE_Comp VALUES(5,'ANUSHKA','SHARMA',20000,'SHARMAA@GMAIL.COM',1,'2021-03-01','IT',NULL);
INSERT INTO EMPLOYEE_Comp VALUES(6,'SOMNATH','MAHARANA',65000,'SMAHA@GMAIL.COM',3,'2019-05-07','IT',1003);

# Write an Query to List all Table Name of database

![image](https://github.com/Official-Vivek-Singh/Most-Commonly-USED-SQL-Query-For-Data-Analyis/assets/129989230/7f529519-f38a-4dcd-bd82-a2f56abd91bd)

# Show all record of Computer Table

select * from COMPUTER;

![image](https://github.com/Official-Vivek-Singh/Most-Commonly-USED-SQL-Query-For-Data-Analyis/assets/129989230/7b878379-bb0f-49fd-bc61-9749db1ded6f)

# Show Record of Employee Table

Select * from EMPLOYEE_Comp;

![image](https://github.com/Official-Vivek-Singh/Most-Commonly-USED-SQL-Query-For-Data-Analyis/assets/129989230/4ea00f2c-abb0-4091-b0f1-dfcfb417a71e)



