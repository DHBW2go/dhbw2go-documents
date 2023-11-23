# Software Requirements Specification

## Table of contents
- [Table of contents](#table-of-contents)
- [Introduction](#1-introduction)
    - [Purpose](#1-1-purpose)
    - [Scope](#1-2-scope)
    - [Definitions, Acronyms and Abbreviations](#1-3-definitions-acronyms-and-abbreviations)
    - [References](#1-4-references)
    - [Overview](#1-5-overview)
- [Overall Description](#2-overall-description)
    - [Vision](#2-1-vision)
    - [Use Case Diagram](#2-2-use-case-diagram)
    - [Technology Stack](#2-3-technology-stack)
- [Specific Requirements](#3-specific-requirements)
    - [Functionality](#3-1-functionality)
    - [Usability](#3-2-usability)
    - [Reliability](#3-3-reliability)
    - [Performance](#3-4-performance)
    - [Supportability](#3-5-supportability)
    - [Design Constraints](#3-6-design-constraints)
    - [Online User Documentation and Help System Requirements](#3-7-on-line-user-documentation-and-help-system-requirements)
    - [Purchased Components](#3-8-purchased-components)
    - [Interfaces](#3-9-interfaces)
    - [Licensing Requirements](#3-10-licensing-requirements)
    - [Legal, Copyright And Other Notices](#3-11-legal-copyright-and-other-notices)
    - [Applicable Standards](#3-12-applicable-standards)
- [Supporting Information](#4-supporting-information)

## 1. Introduction

### 1.1 Purpose
This Software Requirements Specification (SRS) describes all specifications for the web application "YouAndMEME". It includes an overview about this project and its vision, detailed information about the planned features and boundary conditions of the development process.


### 1.2 Scope
The project is going to be realized as an web application.

Actors of this App are the users.

Planned Subsystems are:
* Account System:
  Users have to create accounts so they are able to upload memes. User data must be stored alongside the posting data.

* Storing Data:
  User data for accounts and possibly profiles has to be stored. The data storage will form the foundation for the visualization, account system.

### 1.3 Definitions, Acronyms and Abbreviations
| Abbrevation | Explanation                            |
| ----------- | -------------------------------------- |
| SRS         | Software Requirements Specification    |
| UC          | Use Case                               |
| n/a         | not applicable                         |
| tbd         | to be determined                       |
| UCD         | overall Use Case Diagram               |
| FAQ         | Frequently asked Questions             |

### 1.4 References

| Title                                                              | Date       | Publishing organization   |
| -------------------------------------------------------------------|:----------:| ------------------------- |
| [YouAndMEME Blog](https://blog.youandmeme.de/)    | 20.10.2022 | YouAndMEME Team    |



### 1.5 Overview
The following chapters provide an overview of this project with vision and Overall Use Case Diagram. The third chapter (Requirements Specification) delivers more details about the specific requirements in terms of functionality, usability and design parameters. Finally there is a chapter with supporting information.

## 2. Overall Description

### 2.1 Vision
True to the motto “a meme a day keeps the doctor away”, YouAndMEME has the vision to deliver a daily meme-content. To achieve this we want to create a web-app for viewing and sharing memes with people from all over the world. We want the users to be able to post their own memes and give them the possibility to view, like and comment memes from other users. This can only be successful if we can encourage users to be active. Therefore we plan to create a point-system where a user can gain points for uploading memes, getting likes on the uploaded memes and also for liking memes of other users.

### 2.2 Use Case Diagram

- Green: Planned till end of december
- Blue: Planned till end of june

### 2.3 Technology Stack
The technology we use is:

Backend:
- Spring Boot (Java REST-API Framework)
- MariaDB (SQL Database Platform)

Frontend:
- Angular

IDE:
- IntelliJ
- WebStorm

Project Management:
- JetBrains Space

Deployment:
- Maven Repository

Testing:
- jUnit
- Cucumber
- Jasmine, Karma

## 3. Specific Requirements

### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.  
Until December we plan to implement:
- 3.1.1 Uploading a meme
- 3.1.2 Viewing a meme
- 3.1.3 Creating an account
- 3.1.4 Deleting an account
- 3.1.5 Logging in
- 3.1.6 Logging out

Until June, we want to implement:
- 3.1.6 Liking/Disliking a meme
- 3.1.7 Leveling up
- 3.1.8 Earning Titles

#### 3.1.1 Uploading a meme
This feature is one of the essential ones of our project. The user gets the possibility to upload a meme. Therefore, they have to select a image on their PC or mobile phone and set a title. Afterwards the user has to press the upload button and the meme will be published.

#### 3.1.2 Viewing a meme
This feature is the other core feature and provides a page(most likely the main page) where the users sees a random meme which he can like or dislike or do nothing at all.

#### 3.1.3 Creating an account
To identify all users we need an account system. This account system enables us to build important functions such as keep track of the levels and be able to identify users which keep on uploading memes againts the rules.

#### 3.1.4 Logging in
The app will provide the possibility to register and log in. This will also make the usability easier when a user wants to see his uploaded/liked memes or keep track of his level progress.

#### 3.1.5 Logging out
In case you have multiple accounts or just want to be cautious about your privacy you should be able to manually log out.

#### 3.1.6 Liking/Disliking a meme
There is a possibility to like or dislike a meme depending on whether you like it or not.

#### 3.1.7 Leveling up
We are implementing a level feature for our users that distributes experience to active users for uploaded memes and distributed likes/dislikes.

#### 3.1.8 Earn Titles
The user gets also the possibility to earn titles for special achievments depending on their level and activity.


### 3.2 Usability
We plan on designing the user interface as intuitive and self-explanatory as possible to make the user feel as comfortable as possible using the web app. Though an FAQ document will be available, it should not be necessary to use it.

#### 3.2.1 No training time needed
Our goal is for a user to open the website and be able to use all the features without any explanation or help.

#### 3.2.2 Familiar Feeling
We want to implement an web app with familiar designs and functions. This way the user is able to interact in familiar ways with the web app without having to get to know new interfaces.

### 3.3 Reliability

#### 3.3.1 Availability
The server shall be available 95% of the time. This also means we have to figure out the "rush hours" of our web app because the downtime of the server is only tolerable when as few as possible players want to use the app.

#### 3.3.2 Defect Rate
Our goal is that we have no loss of any data. This is important this is important to satisfy the users.

### 3.4 Performance

#### 3.4.1 Capacity
The system should be able to manage thousands of requests. Also it should be possible to register as many users as necessary. The data storage should offer the possibility to store more than 10000 images.

#### 3.4.3 App performance / Response time
To provide the best web performance we aim to keep the request and response time as low as possible. To shorten loading times we try to load only the content that is currently needed. This will make the user experience much better.

### 3.5 Supportability

#### 3.5.1 Coding Standards
We are going to write the code by using all of the most common clean code standards. For example we will name our variables and methods by their functionalities. This will keep the code easy to read by everyone and make further developement much easier.

#### 3.5.2 Testing Strategy
The application will have a high test coverage and all important functionalities and edge cases should be tested. Further mistakes in the implementation will be discovered instantly and it will be easy to locate the error.

### 3.6 Design Constraints
We are trying to provide a modern and easy to handle design for the UI aswell as for the architecture of our application. To achieve that the functionalities will be kept as modular as possible.

Because we are programming an web application we chose Java for our backend and Angular for our frontend. Also we are using the common MVC-architecture to keep the frontend and backend separated.
To make the communication between the two parts easy, we will implement a RESTful-API between them which will provide the data in JSON-Format.

### 3.7 Online User Documentation
The usage of the web app should be as intuitive as possible so it won't need any further documentation.

### 3.8 Purchased Components
We don't have any purchased components yet. If there will be purchased components in the future we will list them here.

### 3.9 Interfaces

#### 3.9.1 User Interfaces
The User interfaces that will be implented are:
- Dashboard - view all memes by scrolling through your feed
- Login - this page is used to log in
- Register - provides a registration form
- Profile - makes it possible to set a profile picture, post information about yourself

#### 3.9.2 Hardware Interfaces
(n/a)

#### 3.9.3 Software Interfaces
The web app will be available on all common internet browsers.

#### 3.9.4 Communication Interfaces
The server and client will communicate using the http protocol.

### 3.10 Licensing Requirements

### 3.11 Legal, Copyright, and Other Notices
The logo is licensed to the YouAndMEME Team and is only allowed to use for the application. We do not take responsibilty for any incorrect data or errors in the application.

### 3.12 Applicable Standards
The development will follow the common clean code standards and naming conventions. Also we will create a definition of d which will be added here as soon as its complete.

## 4. Supporting Information
For any further information you can contact the YouAndMEME Team or check our [YouAndMEME Blog](https://blog.youandmeme.de/).
The Team Members are:
- Jolina Heesen
- Dennis Rayker
- Maximilian Bräuer
- Kai Beisheim