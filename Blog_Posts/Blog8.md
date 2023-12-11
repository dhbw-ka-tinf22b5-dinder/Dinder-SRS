# Architectural goals and constraints
### Architectural Goals
- We want modularity so we can easily implement new features. We ensure this by using Springboot. With this framework we are able to easily create new api endpoints. OpenAPI and redoc then create an api-     specification for the new endpoint automatically.
- The backend does all the logic while our frontend acts only as an interface to the api. Thus we would also be able to create an Android or IOS-App very easily in the future. 
- We currently don’t use test driven development but we will write tests in the future 

### Constraints
- We develop this as pure webapp timeframe till end of 4th semester.
- We use React because we have the most experience in this framework.
- It is mandatory to use free tools and hosting providers. 
- Our experience with building webprojects is limited
# Process view
These diagrams describe the basic processes of the application

[chat_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/ChatDinder.png)

[login page_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/loginPageSource.png)

[registration page_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/registrationPage.png)

[search_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/search.png)

[swipe_Sequence](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/tree/main/Diagramme/Sequenzdiagramme/swipe.png)

[class diagram backend](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Klassendiagramme/Backend.png)

[class diagram frontend](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Klassendiagramme/Frontend.png)
# Implementation view
![componentDiagram](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/assets/48451580/ce83cbed-08e8-41e3-8a37-3102a8f13437)
## Overview
- Database
- backend
    - Since we use the MVC-pattern the backend handels the logic
    - It connects to the database with springboot
- frontend
    - It only displays the data given by the backend
    - It connects to the backend via http
## Layers
- backend:
  - controller : endpoints of the api
  - services : handles logic
  - repositories : connect to database
- frontend
  - http-client : sends requests for data to the backend
  - redux : saves the data in states
  - webpage : displays the data
# Quality
- Extensibility : 
    - modular design : We try to keep featrures seperated from each other, so we can easily modify them without changing everything
- portability : 
    - MVC-pattern : All the logic is in the backend, thus we only have to rewrite the frontend
    - React : The frontend is written in react with typescript. This helps to port the code to other typescript frontends like react-native.
- security :
    - JWT : The token is stored as a cookie so it is hard for attackers to steal it
