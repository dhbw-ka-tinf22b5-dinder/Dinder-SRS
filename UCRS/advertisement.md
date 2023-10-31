
## Use-Case-Realization Specification: Advertisement

1. Introduction
    1. Purpose

       Der Zweck dieses Use Cases ist, eine neue Anzeige für eine Dienstleistung zu erstellen mit vorgegebenen Merkmalen.
    
    2. Scope

       Insbesondere der Use Case "find work" und "work (chat)" ist direkt mit dem beschriebenen Use Case verbunden, da die beiden Use Cases ohne den hier beschriebenen nicht funktionieren.
    
    3. Definitions, Acronyms, and Abbreviations

       wird bedarfsweise erstellt

    4. References
   
       [GUI Mockup](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/MockUps/MockUp-Advertisement.pdf)
       
       [Sequenzdiagramm](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Sequenzdiagramme/FormPageAdvertisement.png)

       [SRS](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/SoftwareRequirementsSpecification.md)


2. Flow of Events - Design

![Sequence Diagram](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder-SRS/blob/main/Diagramme/Sequenzdiagramme/FormPageAdvertisement.png)

Request From Page:

- Die Seite wird vom User angefragt und der Server schickt die Webseite an den User.
    
Fill out Form, Submit Form:

- Der User füllt die Eingabefelder zur Erstellung einer Anzeige aus und bestätigt seine Eingabe. Diese wird dann an den Server geschickt.

Save Advertisement Data:

- Nach Validierung der Eingaben durch den Server werden die Informationen an die Datenbank geschickt, wobei nach Erfolg die Datenbank eine Bestätigung an den Server sendet. 

Advertisement Added:

- Der Webserver schickt die Bestätigung/Fehlermeldung an den User

View Advertisement:

- Nach erfolgreicher Erstellung kann der User sich seine erstellten Aktivitäten durch Server-User-Kommunikation
 anschauen
