# Building WPF and ASP.NET Applications with Entity Framework

This tutorial shows how to build a WPF(desktop) application and a ASP.NET(web) application that displays data from a SQL Server database. 

# Starter Steps for Both WPF and ASP.NET Apps

### 1. Make Database with Fake Data

Let's call this project "Venme." We first start a SQL Server (localhost) database called "Venme." We make two tables, "User" and "Transaction." 

### 1. Add Primary Key

**Important**: declare primary key for `id`. Otherwise the following steps will break.

Insert some fake data using the following:

If you cannot change the table design


# . ASP.NET Web App

### 1. Generate Models from Database with Entity Framework

Assume you completed the starter step "Make Database with Fake Data," now right click on your project > click "Add" > click "New Item."

In the popup menu, select "Entity Framework," and name it "VenmeContext"

### 1. Migrate Data
PMC > enable-migrations -VenmeContext


### 1. (Optional) 

### 1. Move model files into the Models folder







### 1. Add Controllers


### 1. Edit Views to Display Data
