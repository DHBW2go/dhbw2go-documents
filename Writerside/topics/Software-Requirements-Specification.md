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
    - [Purchased Components](#3-8-purchased-components)
    - [Interfaces](#3-9-interfaces)
    - [Licensing Requirements](#3-10-licensing-requirements)
    - [Legal, Copyright And Other Notices](#3-11-legal-copyright-and-other-notices)
    - [Applicable Standards](#3-12-applicable-standards)
- [Supporting Information](#4-supporting-information)

## 1. Introduction
### 1.1 Purpose
This Software Requirements Specification (SRS) describes all specifications for the native application "DHBW2go". It 
includes an overview about this project and its vision, detailed information about the planned features and boundary conditions of the development process.


### 1.2 Scope
The project is going to be realized as a native application.

Actors of this App are the users.

Planned Subsystems are:
* Account System:
  Users have to create accounts so they are able to customize the app. 

* Storing Data:
  User data for accounts and possibly profiles has to be stored. The data storage will form the foundation for the account system.

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

| Title                                         |    Date    | Publishing organization |
|-----------------------------------------------|:----------:|-------------------------|
| [DHBW2go GitHub](https://github.com/DHBW2go) | 06.02.2024 | DHBW2go Team            |



### 1.5 Overview
The following chapters provide an overview of DHBW2go with vision and Overall Use Case Diagram. The third chapter 
(Requirements Specification) delivers more details about the specific requirements in terms of functionality, usability and design parameters. Finally there is a chapter with supporting information.

## 2. Overall Description

### 2.1 Vision

Our vision is to create a mobile application tailored to the needs of students at the Baden-Württemberg Cooperative State University (DHBW). By combining state-of-the-art technologies with an intuitive, user-friendly interface, we aim to revolutionize students' daily academic routines and enhance their organization and efficiency.

The software will not just be another app; it will serve as a comprehensive solution to help students better manage and structure their university tasks and obligations. This includes displaying class schedules, managing exam grades, and integrating other relevant academic information. However, our vision extends beyond mere functionality – we aim to build a platform that simplifies and enriches academic life at DHBW.

### 2.2 Use Case Diagram

![Use Case Diagram](https://github.com/DHBW2go/dhbw2go-documents/blob/main/Diagramme/UseCase_Diagramm.png?raw=true)

### 2.3 Technology Stack
The technology we use is:

Backend:
- Spring Boot

Frontend:
- React Native

IDE:
- IntelliJ IDEA Ultimate

Project Management:
- GitHub Projects

Deployment:
- tbd

Testing:
- tbd

## 3. Specific Requirements

### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.  


#### 3.1.1 Use-Case
Specify use-cases per subsection.


### 3.2 Usability
We plan on designing the user interface as intuitive and self-explanatory as possible to make the user feel as 
comfortable as possible using the native app. 

#### 3.2.1 No training time needed
Our goal is for a user to open the application and be able to use all the features without any explanation or help.

#### 3.2.2 Familiar Feeling
We want to implement a native app with familiar designs and functions. This way the user is able to interact in 
familiar ways with the native app without having to get to know new interfaces.

### 3.3 Reliability

#### 3.3.1 Availability
The server shall be available 95% of the time. This also means we have to figure out the "rush hours" of our native app 
because the downtime of the server is only tolerable when as few as possible users want to use the app.

#### 3.3.2 Defect Rate
Our goal is that we have no loss of any data. This is important to satisfy the users.

### 3.4 Performance

#### 3.4.1 Capacity
The system should be able to manage thousands of requests. Also it should be possible to register as many users as necessary. 

#### 3.4.3 App performance / Response time
To provide the best performance we aim to keep the request and response time as low as possible. To shorten loading times we try to load only the content that is currently needed. This will make the user experience much better.

### 3.5 Supportability

#### 3.5.1 Coding Standards
We are going to write the code by using all the most common clean code standards. For example, we will name our 
variables and methods by their functionalities. This will keep the code easy to read by everyone and make further development much easier.

#### 3.5.2 Testing Strategy
The application will have a high test coverage and all important functionalities and edge cases should be tested. Further mistakes in the implementation will be discovered instantly and it will be easy to locate the error.

### 3.6 Design Constraints
We are trying to provide a modern and easy to handle design for the UI as well as for the architecture of our 
application. To achieve that the functionalities will be kept as modular as possible. To keep a constant design, we 
use libraries for the styling of the UI.

### 3.7 Online User Documentation
The usage of the native app should be as intuitive as possible, so it won't need any further documentation.

### 3.8 Purchased Components
We don't have any purchased components yet. If there will be purchased components in the future we will list them here.

### 3.9 Interfaces

#### 3.9.1 User Interfaces
The User interfaces that will be implented are:
- Dashboard 
- Login - this page is used to log in
- Register - provides a registration form
- Profile - makes it possible to set your course 

#### 3.9.2 Hardware Interfaces
(n/a)

#### 3.9.3 Software Interfaces
The native app will be available on iOS and Android Platforms.

#### 3.9.4 Communication Interfaces
tbd

### 3.10 Licensing Requirements
(n/a)

### 3.11 Legal, Copyright, and Other Notices
The logo is licensed to the DHBW. We do not take responsibility for any incorrect data or errors in the application.

### 3.12 Applicable Standards
The development will follow the common clean code standards and naming conventions. Also, we will create a definition of d which will be added here as soon as its complete.

## 4. Supporting Information
For any further information you can contact the DHBW2go Team (E-Mail: info@dhbw2go.de)

The Team Members are:
- Jolina Heesen
- Kai Beisheim