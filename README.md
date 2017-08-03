# Building WPF and ASP.NET Applications with Entity Framework

This tutorial shows how to build a WPF(desktop) application and a ASP.NET(web) application that displays data from a SQL Server database. 

# Starter Steps

### 1. Make Database with Fake Data

Let's call this project "Venme." We first start a SQL Server (localhost) database called "Venme." You have two tables, one called "User" and the other "Transaction." Insert some fake data using the following:

# . ASP.NET Web App

### 1. Add Database Connection

Assume you completed the starter step "Make Database with Fake Data," now right click on your project > click "Add" > click "New Item."

In the popup menu, select "Entity Framework," and name it "VenmeContext"
