# Dinder - Software Requirements Specification

## Table of contents
- [Table of contents](#table-of-contents)
- [Introduction](#1-introduction)
    - [Purpose](#11-purpose)
    - [Scope](#12-scope)
    - [Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)
    - [References](#14-references)
    - [Overview](#15-overview)
- [Overall Description](#2-overall-description)
    - [Vision](#21-vision)
    - [Use Case Diagram](#22-use-case-diagram)
    - [Technology Stack](#23-technology-stack)
- [Specific Requirements](#3-specific-requirements)
    - [Functionality](#31-functionality)
    - [Usability](#32-usability)
    - [Reliability](#33-reliability)
    - [Performance](#34-performance)
    - [Supportability](#35-supportability)
    - [Design Constraints](#36-design-constraints)
    - [Online User Documentation and Help System Requirements](#37-on-line-user-documentation-and-help-system-requirements)
    - [Purchased Components](#38-purchased-components)
    - [Interfaces](#39-interfaces)
    - [Licensing Requirements](#310-licensing-requirements)
    - [Legal, Copyright And Other Notices](#311-legal-copyright-and-other-notices)
    - [Applicable Standards](#312-applicable-standards)
- [Supporting Information](#4-supporting-information)

## 1. Introduction

### 1.1 Purpose
This document serves as the Software Requirements Specification (SRS) for the "Dinder" application, comprehensively delineating the specifications associated with the project. Within these pages, you will find an introductory discourse on the project's objectives and overarching vision, as well as in-depth insights into the anticipated features and the parameters that define the development process.

### 1.2 Scope
The project is going to be realized as a Web Application.

Actors of this App are Users. These users have the roles of contractor or a employer.

Planned Subsystems are:
* Login page:  
  Users can log in and register.
* main page:  
  Users can view the services they want to work on
* Advertisement creation:  
  Users can create an advertisement for services for others to work on
* Chat:  
  contractor and employer chat to discuss details and pricing
*  Account System:  
   Users can create accounts, so they can accept a service advertisement. User data must be stored alongside the posting data.
* Swiping:
  Similar to Tinder, the User should be able to swipe through open service advertisements
* Connecting People:  
  The person who posts an available service task must be notified if someone wants to complete the service task. Both must then be able to get in touch to organize the details, so messages between the host and the guest have to be enabled. This will be done with a chat function. For this an account system is needed.
* Storing Data:  
  User data for accounts and possibly profiles has to be stored. Also, the service tasks have to be stored as datasets containing the form contents and possibly contact data. The data storage will form the foundation for the visualization, account system and the search feature.


### 1.3 Definitions, Acronyms and Abbreviations
| Abbrevation | Explanation                         |
|-------------|-------------------------------------|
| SRS         | Software Requirements Specification |
| UC          | Use Case                            |
| n/a         | not applicable                      |
| tbd         | to be determined                    |
| UCD         | overall Use Case Diagram            |
| FAQ         | Frequently asked Questions          |

### 1.4 References

| Title                                                                                               |    Date    | Publishing organization |
|-----------------------------------------------------------------------------------------------------|:----------:|-------------------------|
| [Dinder Blog](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder/discussions/categories/projektblog) | 17.10.2023 | Dinder                  |
| [GitHub](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder/)                                        | 17.10.2023 | Dinder                  |


### 1.5 Overview
The following chapter provides an overview of this project with vision and Overall Use Case Diagram. The third chapter (Requirements Specification) delivers more details about the specific requirements in terms of functionality, usability and design parameters. Finally, there is a chapter with supporting information.

## 2. Overall Description

### 2.1 Vision
Inspired by offering platforms like ‘Ebay’ and ‘Kleinanzeigen’ we wanted to build an application that simplifies the process of finding a helping hand as much as ‘Tinder’. We plan to create a platform for people who are looking for someone to help with work.
To enable anyone to browse the available jobs, such as babysitting, gardening or painting, the widely known Tinder interface will be used. Users can swipe left and right on available Service tasks.

### 2.2 Use Case Diagram

![UC](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/UseCaseDiagram.png)


### 2.3 Technology Stack
The technology we use is:

### Web-App

#### Backend:
- Gradle
- Spring Boot
- MariaDB

### Frontend:
- React

#### IDE:
- IntelliJ
- Eclipse

#### Project Management:
- YouTrack
- GitHub
- Discord

#### Deployment:
- Travis CI
- Docker and Heroku

#### Testing:
- Cucumber
- Espresso
- JUnit
- Codacy
- CodeMR
- RestAssured

## 3. Specific Requirements

### 3.1 Functionality
This section will explain the different use cases, you could see in the Use Case Diagram, and their functionality.


#### 3.1.1 Creating an account
To identify all useres we need an account system. This account system enables us to build important functions.

Sequence diagram:
![register_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/registrationPage.png)

Activity Diagram:

UCRS: ![ucrs registration](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/UCRS/registration.md)

#### 3.1.2 Logging in
The app will provide the possibility to register and log in.

Sequence diagram:
![login_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/loginPageSource.png)

Activity Diagram:

#### 3.1.3 Form page for a new advertisement / edit an existing advertisement
There is the possibility to fill out a form page to create a new service advertisement.

Sequence Diagram:
![form page_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/FormPageAdvertisement.png)

Activity Diagram:

UCRS (new advertisement): ![ucrs new advertisement](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/UCRS/advertisement.md)

#### 3.1.4 Swiping
The user can similar to Tinder swipe through open service advertisements and chose his preferred tasks.

Sequence Diagram:
![swipe_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/swipe.png)

Activity Diagram:
#### 3.1.5 Search function for open service advertisements
The user can use a search function with individual filters (ex.: Distance)

Sequence Diagram:
![search_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/search.png)

Activity Diagram:
#### 3.1.6 Chat function
The user and the advertiser are able to exchange Details about the task in a private chat

Sequence Diagram:
![chat_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/ChatDinder.png)

Activity Diagram:
### 3.2 Usability
We plan on designing the user interface as intuitive and self-explanatory as possible to make the user feel as comfortable as possible using the website. Though an FAQ document will be available, it should not be necessary to use it.

#### 3.2.1 No training time needed
Our goal is that a user opens the Web application and is able to use all features without any explanation or help.

#### 3.2.2 Familiar Feeling
We want to implement an website with familiar designs and functions. This way the user is able to interact in familiar ways with the Web app without having to get to know new interfaces.


### 3.3 Reliability

#### 3.3.1 Availability
The server shall be available 95% of the time. This also means we have to figure out the "rush hours" of our app because the downtime of the server is only tolerable when as few as possible players want to use the app.

### 3.4 Performance

#### 3.4.1 Capacity
The system should be able to manage thousands of requests. Also it should be possible to register as many users as necessary.


#### 3.4.2 Web App perfomance / Response time
To provide the best App perfomance we aim to keep the response time as low as possible. This will make the user experience much better.

### 3.5 Supportability

#### 3.5.1 Coding Standards
We are going to write the code by using all of the most common clean code standards. For example we will name our variables and methods by their functionalities. This will keep the code easy to read by everyone and make further developement much easier.

#### 3.5.2 Testing Strategy
The application will have a high test coverage and all important functionalities and edge cases should be tested. Further mistakes in the implementation will be discovered instantly, and it will be easy to locate the error.

### 3.6 Design Constraints
We are trying to provide a modern and easy to handle design for the UI aswell as for the architecture of our application. To achieve that the functionalities will be kept as modular as possible.

We are using the common MVC-architecture to keep the front end and back end seperated. For a clean front end structure we use MVVM.
For the Front End we will use React.


### 3.7 On-line User Documentation and Help System Requirements
The usage of the Web app should be as intuitive as possible so it won't need any further documentation. If the user needs some help we will implement a "Help"-Button in the App which includes a FAQ and a formular to contact the developement team.

### 3.8 Purchased Components
We don't have any purchased components yet. If there will be purchased components in the future we will list them here.

### 3.9 Interfaces

#### 3.9.1 User Interfaces
The User interfaces that will be implemented are:
- Dashboard - lists all open service advertisements
- Swiping - Makes it possible to swipe though service advertisements
- Search - Makes it possible to search service advertisements
- Service advertisements Creation - Makes it possible to crate new service advertisements
- Login - this page is used to log in
- Register - provides a registration form
- Profile - Shows the stats of your completed tasks
- Settings - shows the settings, Changing Password, Email and profile picture is possible

#### 3.9.2 Hardware Interfaces
(n/a)

#### 3.9.3 Software Interfaces
In the first Stage it will be a Web App. In the Future an Android App is possible

#### 3.9.4 Communication Interfaces
The server and hardware will communicate using the http protocol.

### 3.10 Licensing Requirements

### 3.11 Legal, Copyright, and Other Notices
The logo is licensed to the Common Playground Team and is only allowed to use for the application. We do not take responsibilty for any incorrect data or errors in the application.

### 3.12 Applicable Standards
The development will follow the common clean code standards and naming conventions. Also we will create a definition of d which will be added here as soon as its complete.

## 4. Supporting Information

The Team Members are:
- Jannis Fuchs (Frontend)
- Lukas Schulz (Frontend)
- Jonathan Schäfer (Backend)
- Tobias Raible (Backend)
- Manuel Franz (Database)

<!-- Picture-Link definitions: -->
[OUCD]: https://github.com/IB-KA/CommonPlayground/blob/master/UseCaseDiagramCP.png "Overall Use Case Diagram"


## Dinder - GUI Mockup

[Main page](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Main.pdf)
