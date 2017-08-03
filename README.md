# Building WPF and ASP.NET Applications with Entity Framework

This tutorial shows how to build a WPF(desktop) application and a ASP.NET(web) application that displays data from a SQL Server database. 

# Starter Steps for Both WPF and ASP.NET Apps

### 1. Make Database with Fake Data

Create a database called 'Venme'.

Make two tables, "User" and "Transaction" with the following script:

```sql
USE Venme;

CREATE TABLE Users (
	id int Primary Key,
	name varchar(255) NOT NULL
);

CREATE TABLE Transactions (
	id int Primary Key,
	[from] int,
	[to] int,
	amount int
);
```

Insert some fake data for "Users":

```sql
USE Venme;
GO

INSERT INTO [Users] VALUES 
	(1, 'Marvin Minsky'), 
	(2, 'John McCarthy'), 
	(3, 'Edsger Dijkstra'), 
	(4, 'Donald Knuth'), 
	(5, 'Allen Newell'), 
	(6, 'Herbert Simon');
```



Some fake data for 'Transactions':

```sql
USE Venme;
GO

INSERT INTO [Transactions] VALUES 
	(1, 1, 2, 35), 
	(2, 1, 3, 24), 
	(3, 2, 4, 7), 
	(4, 3, 5, 56), 
	(5, 4, 1, 89), 
	(6, 6, 5, 45),
	(7, 2, 1, 102), 
	(8, 3, 1, 23), 
	(9, 4, 2, 65), 
	(10, 5, 3, 82), 
	(11, 1, 4, 58), 
	(12, 5, 6, 79);
```




# . ASP.NET Web App

### 1. Generate Models from Database with Entity Framework

Assume you completed the starter step "Make Database with Fake Data," now right click on your project > click "Add" > click "New Item."

In the popup menu, select "Entity Framework," and name it "VenmeContext"

### 1. Migrate Data
PMC > enable-migrations -VenmeContext

### 1. (Optional) Add Primary Key

**Important**: declare primary key for `id`. Otherwise the following steps will break.

Insert some fake data using the following:

If you cannot change the table design

### 1. Move model files into the Models folder







### 1. Add Controllers


### 1. Edit Views to Display Data
