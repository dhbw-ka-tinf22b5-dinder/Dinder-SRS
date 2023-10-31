
## Use-Case-Realization Specification: Registration


1. Introduction
    1. Purpose

       The purpose of this use case is to let the user create an account.
    
    2. Scope
  
       Only after this use case has been completed can the remaining use cases be used.
    
    3. Definitions, Acronyms, and Abbreviations

       to be defined

    4. References
   
       [GUI Mockup](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/MockUps/MockUp-Registration.pdf)
       
       [Sequenzdiagramm](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Sequenzdiagramme/registrationPage.png)

       [SRS](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/SoftwareRequirementsSpecification.md)


2. Flow of Events - Design

![Sequence Diagram](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Sequenzdiagramme/registrationPage.png)

Request From Page:

- The page is requested by the user and the server sends the web page to the user.
    
Fill out Form, Submit Form:

- The user fills in the input fields to create an ad and confirms his input. This is then sent to the server.

Save Advertisement Data:

- After validation of the input by the server, the information is sent to the database, and after success the database sends a confirmation to the server. 

Advertisement Added:

- The web server sends the confirmation/error message to the user.

View Advertisement:

- After successful creation, the user can view his created activities through server-user communication view
