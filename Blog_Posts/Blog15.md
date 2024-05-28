# CI/CD

## Pipeline
*Grobe Beschreibung der Funktion*
- @jonathan: Pipeline um automatisch zu builden + SonarCloud Reports

Nach erfolgreichem durchlaufen der geschriebenen Test wird automatisch ein Artefakt in github actions gebildet. Bei einem fehlerhaften Test wird ein Fehler in der Pipeline angezeigt und die Artefakterstellung wird abgebrochen. Der Pipelineersteller wird daraufhin benachrichtigt. Nach einer erfolgreichen Artefaktbildung kann das Artefakt in der jeweiligen Pipeline im Anhang heruntergeladen werden.

## Konfigurationen
Unsere Pipelines sind auf [GitHub](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder/tree/main/.github/workflows) zu finden:
- Automatischer Formatter: [biome-formatter.yml](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder/blob/main/.github/workflows/biome-formatter.yml)
- Biome Linter: [biome-linter.yml](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder/blob/main/.github/workflows/biome-linter.yml)
- SonarCube + Build: [build.yml](https://github.com/dhbw-ka-tinf22b5-dinder/Dinder/blob/main/.github/workflows/build.yml)

## Sonstige Neuerungen
Im Frontend wurde teils die Dateiorganisation angepasst, sodass sie modularer gestaltet ist. Zusätzlich gibt es jetzt, je nach Webseitenbereich, auch eine diversifizierte Navigationsbar.
