### Frontend

We began to work on the Main Page Component. The typical Tinder-Swipe functionality will be implemented on this Page.
Contractors, who are loking for work, can swipe through available service advertisements. 
For each advertisment a short description will be displayed. There will be ,,Next'', ,,Previous'' and ,,Accept'' Buttons.

- [Screenshot Mainpage 1](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/MockUps/ScreenshotMainPage1.jpg)
- [Screenshot Mainpage 2](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/MockUps/ScreenshotMainPage2.jpg)

We implemented states with redux and added and API-connection to the backend, which can register and validate users.
The states also manage errormessages.
- [email verification](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/assets/48451580/0c14a755-0c1c-473f-95db-0cd5c070de52)
- [passwords don't match](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/assets/48451580/51b14c95-9fd0-4167-9e86-0fe6363660d2)

### Backend

In addition to the Users table, the other tables have been updated and adapted to the rest of the backend.
Additionally, we have improved the connection with the database to include all needed entities in Hibernate.
As an extra feature, we have added an API-Documentation using Redoc (https://github.com/Redocly/redoc) to improve the compatibility with the frontend and to make communication more easy for both sides.

### Distribution of tasks
Jannis - 

Jonathan - Implemented the Hibernate entities and REST-endpoints to access them

Lukas - Creation of a Mainpage, which has the typical Tinder-Swipe function

Manuel - Database (update database tables)

Tobias - Implementation of Redoc, support in implementation of the Hibernate entities
