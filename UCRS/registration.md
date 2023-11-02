
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

enter user data:

- The user enters their user details on the registration page.
    
checks if passwords comply with requirements:

- The web app server checks the password if it meets our password requirements.

check for duplicate account:

- The web app server sends query to the database to check for duplicate accounts. 

send confirmation / send error message:

- If there is no duplicate account, the database will send a confirmation; if there is, it will send an error message.

makes new database entry:

- the web app server sends a SQL command to the database to add a new user to the database

send and display confirmation:

- the database sends a confirmation to the web app server which sends it to the user

display error message and clear password:

- If the password doesn't meet the requirements, the server displays an error message to the user and clears the password fields in the frontend.
