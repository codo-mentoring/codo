<div align="center"><img src="attachments/SiteSettings:global/logo.png"  width="30%"></div>

# codo
*Das Daten-Tool für Mentoringprojekte*

codo basiert auf dem Open Source System der Case Management Plattform [Aam Digital](https://github.com/Aam-Digital/ndb-core).
Im dortigen Repository finden sich Source Code und technische Details: https://github.com/Aam-Digital/ndb-core

Wir werden zukünftig weitere technische Dokumentation und Konfigurationen hier veröffentlichen.

Allgemeine Details zum Projekt: [codo-mentoring.org](https://codo-mentoring.org/)

-----
## Installation des Systems
_codo_ muss von einem Server-Administrator eingerichtet werden und wird dann einfach über einen Webbrowser benutzt.

Die Installation erfordert zunächst die Einrichtung einer Instanz der _Aam Digital_ Plattform.
Diese kann anschließend sehr einfach als _codo_ Systen konfiguriert werden.

### Plattform Setup
wie hier beschrieben: https://github.com/Aam-Digital/ndb-setup/

### Konfiguration als codo System

#### Für Setup-Skript (ndb-setup)
1. Clonen des Setup-Projekts: [Aam-Digital/ndb-setup](https://github.com/Aam-Digital/ndb-setup)
2. Kopieren der Dateien aus diesem Repository hier in das Setup-Projekt unter `baseConfigs/codo`
3. Das Setup-Skript kann jetzt für "codo" ausgeführt werden.

#### Manual im Datenbank-Manager:
1. Aufrufen des Datenbank-Managers "Fauxton": https://<system-url>/db/couchdb/_utils/#
2. Einloggen mit "admin" User und dem während des Setup generierten Passworts (zu finden in der .env Datei auf dem Server)
3. Erstellen eines neuen Dokuments in der "app" Datenbank
4. Kopieren des codo Config files [codo-default-config.json](./entities.json) als Basis-Konfiguration.
5. ggf. weitere Anpassung der Konfiguration
