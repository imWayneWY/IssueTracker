# Issue Tracker (Bug Tracker) System

## 1. Introduction

### 1.1 Purpose
The purpose of this document is to build on issue tracker (bug tracker) system to manage issues and project members to ease the issue management. The main reason to build it is to learn and practice .NET in 2021, and improve my front-end skills as well.

### 1.2 Document Conventions
This docement uses the following conventions.
Abbr | Full Title 
--- | --- 
DB | Database
JS | Javascript
TS | Typescript
RN | React Native
Admin | Administator
Dev | Developer

### 1.3 Intended Audience
This project is a open source demo for tracking issues in a project. It's useful for people who want to deploy a simple issue tracker system in their local enviorment. And also is welcome for anyone who wants to study .NET and React, or modify the code. I will be very appericate if you give me advices and point out my mistakes.

### 1.4 Scope
The purpose of this open source issue tracker management system is to ease the issue management. We will have database to save projects and issues, and also multi-end client for all kinds of platforms. Separation of front-end and back-end will easily support users to log in and manage their projects. I plan to code 1 hours every day, 4 months to build apis using .NET, 4 months to build web application using React, and 3 months to build mobile applications using React-Native. I plan to start this project at the begining of Febrary, and finish it before 2021. Above all, we hope to use this project to track my own projects and share my issues when I build this up. 

## 2. Overall Description
### 2.1 Product Perspective
  Use database to stores the following information.
  + **Projects**

    It includes the information for projects, like the project's name, description.
  + **Users**

    It includes the users' infomation, like name, access type, email, etc.
  + **Issues**
  
    It includes the issues' status, type, title, description, etc.
### 2.2 Product Features
The major database system as hsown in below
![db_design](https://github.com/imWayneWY/IssueTracker/blob/main/DB_Design.png?raw=true)
### 2.3 User Class and Characteristics
Users of the system should be able to track projects and issues' information from the database, and management the projects or issues by their access role type. 

The Admin(Manager) should have all the access to:
  + Create a project
  + Update a project
  + Delete a project
  + Create an issue
  + Delete an issue
  + Change issue's status

The Dev should have the access to:
  + Create an issue
  + Change issue's status

And there also has a visitor who can only view the process of the projects/issues

### 2.4 Operating Environment
This project will use docker to make it easy to deploy. However, Sql Server is still needed.
  + client/server system
  + Database: Sql server
  + Operation system: Any OS which can running docker
  + Api: .NET Core 3.1
  + Web application: Typescript/React
  + Mobile application: Typescript/React-Native
  
## 3. System Features
### 3.1 Functional Requirements
  + Project could been created or removed by Admin
  + Dev could use this system to track the issues
  + Dev could create or close issues
  + Visitors could view the progress of the project
### 3.2 External Interface Requirements
  + All kinds of devices which can use web browser
  + Mobile devices
  + Desktop devices
### 3.3 System Features
  + Windows
  + Macos
  + IOS
  + Android
### 3.4 Nonfunctional Requirements
  + Maintainablity: The Admin should maintain correct project
  + Security: Users can only assess for functions the role is assigned