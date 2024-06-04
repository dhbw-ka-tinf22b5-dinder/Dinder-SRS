# Review
- Datum 4.6.2024
- Startzeit 16:15; Endzeit 17:10
- Teilnehmer :
  - Tobias zeigt Code
  - Kai von Habittracking
  - Jannis Protokoll
  - Manuel und Jonathan moderiert
## Ziel/Fokus :
Das Ziel ist die Qualität in unserem Softwareprojekt zu steigern. Vor allem werden hier die Bereiche betrachtet, die noch entwickelt werden oder einfach zu ändern sind.
- Überprüfung von Backend
  - Datenbankmodells
  - Entities
- Überprüfung von Frontend
  - Migration von React aus NextJS
  - generelle Codequalität
  
## Review-Backend
###  Datenbankmodell 
- SQL-Syntax schön umgesestzt
- ERM ist nicht vollständig -> sollte aktualisiert werden
### Enitities
- werden funktional umgesetzt
- sind über Annotations gut verständlich und übersichtlich
### Generell-Backend
- Nicht einheitliche Sprache : verwendet zum großen Teil Java enthält aber auch kleine Teile Kotlin
- Es gibt Tests die fehlschlagen durch Unterschiede der lokalen Ausführung zur Ausführung in der Pipeline, trotz identischer Versionen

## Review-Frontend
### Migration auf NextJS
- Routing funktioniert nur noch eingeschränkt (Eingabe im Browser-URL)
- Das serverrenderring von NextJS wird nicht verwendet, da das Backend für clientseitiges Rendering ausgerichtet ist

### Code-Beanstandungen
- Spezifizierung von types; statt any spezifischere Typen
- Code könnte vereinfacht werden durch importieren von zusätzlichen Libraries
- Code hat wenig Kommentare, etwas unübersichtlich zu lesen
- Erstellung von zusätzlichen Custom-React-Components könnte den UI-Aufbau vereinfachen
- Erstellung von zusätzlichen Funktionen würde redundanten Code weiter eliminieren
- Kleinigkeiten im CSS, wie das Cursorformat 
  
## Reviewmethodik
- Der Code wurde in den genannten Komponenten genau inspiziert und die Funktionalität der Webanwendung bewertet.

## Kriterien für Review
- Übersichtlichkeit
- Verständlichkeit
- Codequalität


## Ergebnis
Im großen und ganzen macht das Backend einen sehr guten Eindruck trotz kleinerer Probleme
- Fehlerbehebung 
  - ERM vervollständigen
  - die Fehlersuche bei den Tests auswerten
  - die Kotlinverwendung ist allerdings ohne hohen Zusatzaufwand für die Verbindung zur Datenbank notwendig -> Beanstandung akzeptiert
    
Das Frontend macht im großen und ganzen einen guten Eindruck, jedoch sind einzelne Verbesserungen umsetzbar, welche in Zukunft behandelt werden müssen.
 

