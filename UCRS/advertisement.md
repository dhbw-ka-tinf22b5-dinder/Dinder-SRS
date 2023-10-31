
## Use-Case-Realization Specification: Advertisement

1. Introduction
    1. Purpose

       The purpose of this use case is to create a new ad for a service with predefined characteristics.
    
    2. Scope

       In particular, the "find work" and "work (chat)" use cases are directly related to the described use case, since the two use cases do not work without the one described here.
    
    3. Definitions, Acronyms, and Abbreviations

       to be defined

    4. References
   
       [GUI Mockup](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/MockUps/MockUp-Advertisement.pdf)
       
       [Sequenzdiagramm](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Sequenzdiagramme/FormPageAdvertisement.png)

       [SRS](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/SoftwareRequirementsSpecification.md)


2. Flow of Events - Design

![Sequence Diagram](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Sequenzdiagramme/FormPageAdvertisement.png)

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
