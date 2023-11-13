### Class diagram - frontend:
[picture - class diagram frontend](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Klassendiagramme/Frontend.png)

**Description:**
Here's a brief description of the classes and their relationships:

LoginPage: This class represents the page where users can log in. It includes text fields for the username and password, along with a login button.

RegistrationPage: This class represents the page where users can register. It includes text fields for the username, password, password confirmation, and email address.

MainPage: This class represents the main page of the application. It illustrates the typical Tinder system, allowing the contractor to swipe through advertisements.

ChatWindow: This class represents the chat window where users can exchange messages. It includes fields for chat messages and the input field for new messages.

ListedAdvertisements: This class represents a list of listed advertisements. It includes fields for listed ads.

AcceptedAdvertisements: This class represents a list of accepted advertisements. It also includes fields for listed ads.

NavigationBar: This class represents the navigation bar displayed on various pages. It includes buttons to switch between the "Your Chats," "My Listed Advertisements," "User," and "Main Page."

SingleAdvertisement: This class represents a single ad. It includes fields for the ad image, employer name, ad title, date, time, and notes.

### Class diagram - backend:
[picture - class diagram backend](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Klassendiagramme/Backend.png)

**Description:**
A user can both create an advert and apply for others.
Due to the cardinalities, an intermediate table is required for the second option.
Several chats can be assigned to an advertisement, whereby each chat belongs to an advertisement.
A chat consists of any number of messages that are assigned to a specific chat.
A chat is also assigned to two users (contributor, employer), whereby a user can use any number of chats.

The application starts in the DinderApplication class, which then forwards the start call to the spring framework.
This in turn creates all needed instances of the classes in the application.
The repository-classes contain default methods to modify the entities in the database and to find them by an optional criteria.
The Service holds instances of all the repository-classes, it exposes their functionality to all other classes.
It also provides additional functionality that require some logic to be implemented.
The DinderRestController defines the HTTP-endpoints for the application, which allow outside access to see and modify the data.

### Sequence diagrams:

