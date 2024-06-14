### RMM Tabelle

|Risk ID|Category  |Risk Description        |Probability|Impact|Risk Score|Mitigation Strategy                                 |Indicator                   |Contingency Plan                        |Responsible|Status  |Last Modified Date|
|-------|----------|------------------------|-----------|------|----------|----------------------------------------------------|----------------------------|----------------------------------------|-----------|--------|------------------|
|1      |DB        |DB-Server is unavailable|<1%        |HIGH  |3 von 10  |Usage of HA and Fault Tolerance for better stability|no response                 |Transfer to new DB, via Transaction Logs|Manuel     |pending |11. April         |
|2      |Quality   |Bugs in the software    |100%       |HIGH  |9 von 10  |Usage of Tests (so far ~63%), Code Reviews          |unexpected software behavior|Fix the issues                          |All        |pending |13. June          |
|3      |Management|loss of personell       |15%        |HIGH  |6 von 10  |Exchange on critical reviews, exchange of knowledge |Many bad exams              |Reduction of the software               |All        |occurred|14. June          |

### Größtes technologische Risiko
Unser größtes Risiko war schlechte Codequalität (ID 2). Deshalb nutzten wir Peer Reviews und diskutierten unsere Änderungen. Darüber hinaus verwenden wir Testpipelines.
Wir haben uns hierbei diverse Metriken zur Qualitätsüberprüfung ausgesucht und eine Code Coverage Grenze von mind. 51 % gefordert. Mehr dazu steht im Kapitel Qualitätssicherung.
Abschließend kann jedoch gesagt werden, dass wir unter anderem durch die Pipelines Fehler gefunden haben, wodurch das Gesamtrisiko reduziert wurde. Dennoch befindet sich unsere Demo noch nicht in einem fehlerfreien Zustand, was unsere Einstufung des Risikos verdeutlicht.
