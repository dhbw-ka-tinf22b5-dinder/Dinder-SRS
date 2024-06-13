## Clean Code Refactoring

### Frontend
 
Für das Refactoring im Frontend wurde sich an biome.js gehalten. Dabei hat Biome Fehler in mehreren Bereichen gefunden.
Diese waren größtenteils Fehler im Bezug auf:

- Imports, wobei diese alphabetisch sortiert sein sollten und TypeScript Klassen mit dem Schlüsselwort "type" importiert werden sollte
- Formatting, mit folgenden Fehlern: 
    - Redundanz, vor allem bei Semikola, die in JavaScript meist optional sind
    - zu wenig oder zu viele Leerzeichen in genesteten Funktionen, wodurch es unklar wird, auf welchem Level der Code ist, was wiederum zu einer schlechten Lesbarkeit des Codes führt 
    - das Benutzen von `'` anstelle von `"`


### Backend
- Benutzen von Spring Profilen
- In-Memory Datenbank (H2) für lokale Test, die durch die Spring Profile aktiviert werden kann. Dadurch ergeben sich mehrere Vorteile: 
    - es ist keine Internetverbindung mehr nötig, um das Backend auszuführen, dies war vor allem davor durch die Portblockierungen der DHBW schwer 
    - Veränderungen können ausgetestet werden, ohne die Produktivdatenbank mit Daten beim Entwickeln zu befüllen. Dadurch ist gewährleistet, dass auf der Produktivdatenbank nur echte Daten liegen und keine bei der Entwicklung hinzugefügt
- Die Konfiguration der Datenbankverbindung wurde von einer benutzerdefinierten Bean auf die Verwendung der Spring-Autokonfiguration geändert
- Flyway wird jetzt auch durch die Autokonfiguration geladen
- Die Klasse `AuthorityFactory` wurde zu `AuthoritySupplier` umbenannt, um besser den eigentlichen Nutzen der Klasse zu reflektieren