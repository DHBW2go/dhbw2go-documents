# Software Architecture Document

## 1. Introduction
### 1.1 Purpose
This document provides a comprehensive architectural overview of the system,
using a number of different architectural views to depict different aspects of the system.
It is intended to capture and convey the significant architectural decisions which have been made on the system.

### 1.2 Scope
The scope of this SAD is to show the architecture of our project.

### 1.3 References
- [Jetbrains Space](https://youandmeme.jetbrains.space/)
- [Blog](https://blog.youandmeme.de/)
- [Software Requirements Specification](https://youandmeme.jetbrains.space/p/youandmeme/documents/Documentation/a/Software-Requirement-Specification-SRS)

## 2. Architectural Representation
Our application is set up to use a MVC-architecture which looks as follows:



## 3.Architectural Goals and Constraints

We are not using a tool to implement the MVC-architecture. Since we want to learn about the architecture we prefer to implement it by hand.

## 4. Use-Case View


## 5. Logical View

### 5.1 Overview

For our application the logical view looks like:


The following figure shows the structural organization of our application. Referring to the previous figure, the controller is associated with the spec.ts and .ts files, while the view is associated with the .html and .css files.


### 5.2 Architecturally Significant Design Packages

In this section you can find the generated class diagrams for backend and frontend.

This is our backend:

And this is our frontend:

The class diagram shows only a small part of the components, because the complete one is very big and confusing. If you are interested you can find it [here](https://youandmeme.jetbrains.space/p/youandmeme/documents/Documentation/a/ClassDiagramFrontendpng).

## 6. Process View
The process view shows our four main views and the possible interactions the user sees when using our web application.


## 7. Deployment View


## 8. Implementation View

### Overview

YouAndMEME's Implementation View consists of 3 layers:

* Frontend Layer
* Backend Layer
* Database Layer


### New Design Pattern