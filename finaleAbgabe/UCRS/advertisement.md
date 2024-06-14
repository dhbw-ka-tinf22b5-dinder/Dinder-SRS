
## Use-Case-Realization Specification: Advertisement

### Introduction
    1. Purpose

       The purpose of this use case is to create a new advertisement for a service with predefined characteristics.
    
    2. Scope

       In particular, the "find work" use case is directly related to the described use case, since it is not possible to find work without an advertisement
  

### Flow of Events - Design

[Sequence Diagram](../images/Diagramme/Sequenzdiagramme/FormPageAdvertisement.png)

Request From Page:

- The page is requested by the user and the server sends the web page to the user.
    
Fill out Form, Submit Form:

- The user fills in the input fields to create an ad and confirms his input. This is then sent to the server.

Save Advertisement Data:

- After validation of the input by the server, the information is sent to the database, and after success the database sends a confirmation to the server. 

Advertisement Added:

- The web server sends the confirmation/error message to the user.

View Advertisement:

- After successful creation, the user can view his created activities.
