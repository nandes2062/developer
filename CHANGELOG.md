Changelog
=========

Version 3.6.1 – 26.10.2017
--------------------------

* Die Ordnernamen enthielten HTML-Entities ("&amp;" statt "&" etc.)

Version 3.6.0 – 24.10.2017
--------------------------

* Übersetzungen: Verbesserung Englisch, neu Portugiesisch und Schwedisch
* Consolen-Command für das Synchronisieren über die cli
* Hauptpfad kann über `rex_developer_manager::setBasePath()` geändert werden
* Option zum Deaktivieren der Synchronisation im Backend
* Option für ID-Suffix in Ordnernamen
* Option für Erhaltung der Umlaute default inaktiv, Option ist nun deprecated
* Bessere Ersetzung von Umlauten (insbesondere der Nicht-Deutschen)
* Namen beginnend mit "translate:" werden auch im Ordnernamen übersetzt
* Beim Aufruf von Medien über den Media Manager wird die Synchronisation nicht gestartet
* Die mtime der Dateien wird nicht unnötig neu gesetzt (versursachte teilweise Reloadhinweise in manchen Editoren)

Version 3.5.0 – 09.06.2016
--------------------------

* Übertrag zu Friends Of REDAXO
* Synchronisation in Frontend kann deaktiviert werden
* Bugfix: "Module synchronisieren" konnte nicht deaktiviert werden

Version 3.4.1 – 05.05.2016
--------------------------

* Bugfix: Bei paralleler Entwicklung lokal/Server kam es teilweise zum ungewollten Löschen von Sync-Ordnern

Version 3.4.0 – 18.01.2016
--------------------------

* Anpassungen für REDAXO 5 final
* Bugfix: Nach einem DB-Import wurden die Daten teilweise direkt wieder mit Altdaten überschrieben

Version 3.3.1 – 10.05.2014
--------------------------

* Bugfix: In Kombination mit Autoloadern konnte es zu Fehlermeldungen kommen

Version 3.3.0 – 14.02.2013
--------------------------

* Neuer EP: DEVELOPER_MANAGER_START
* Performanceverbesserung
* Bugfix: Unter bestimmten Umständen wurden die Ordner (teilweise auch DB-Einträge) bei jedem Aufruf vervielfältigt

Version 3.2.0 – 08.11.2013
--------------------------

* Min. REDAXO-Version: 4.3.2
* Korrekte Dateinamen (mit Präfix-Option fehlte ein Punkt vor input.php etc.)
* Optional können Umlaute wieder ersetzt werden
* Die Einstellungen wirken sich beim Speichern direkt aus
* Optional können die Ordner- und Dateinamen automatisch aktuell gehalten werden
* Optional können die Item-Ordner automatisch gelöscht werden nach dem Löschen über das Backend

Version 3.1.1 – 14.08.2013
--------------------------

* Die Einstellungen werden außerhalb des Addonordners in /redaxo/include/data/addons/developer gespeichert
* Neuer Standardpfad für die synchronisierten Dateien: /redaxo/include/data/addons/developer

Version 3.1.0 - 03.08.2013
--------------------------

* Parallele Entwicklung für REDAXO 5
* Optional kann allen Dateien ein Präfix bestehend aus ID und Name vorangestellt werden
* Die ID wird im Namen der ID-Datei gespeichert statt im Inhalt ("1.rex_id" etc.)
* PlugIn-Unterstützung
* Umlaute/Sonderzeichen im Namen werden beibehalten, nur wirklich problematische werden ersetzt

Version 3.0.0 – 20.02.2013
--------------------------

* Grunderneuerung (Mindestvoraussetzungen: PHP 5.3.3, REDAXO 4.3)
* Pro Template/Module/Action ein Ordner (dadurch Verwaltung mit git möglich)
* Templates/Module/Actions können über das Dateisystem neu angelegt werden
* Metadaten werden jeweils über eine YAML-Datei verwaltet
* Weitere Synchronisationen können über PlugIns bzw. andere AddOns hinzugefügt werden

Version 2.2.2 – 10.10.2012
--------------------------

* Alle Synchronisierungen standardmäßig aktiviert
* Bugfix: Nach DB-Import wurden Templates/Module direkt wieder mit den vorherigen überschrieben

Version 2.2.1 – 22.03.2011
--------------------------

* Behebung kleinerer Bugs
* Neues Dateinamenschema mit Template/Module-Namen am Anfang für alphabetische Sortierung

Version 2.2.0 – 05.12.2010
--------------------------

* Synchronisation der Actions
* Verbesserte Aufräumarbeiten
* Synchronisation erst nach ADDONS_INCLUDED

Version 2.1.0 – 19.11.2010
--------------------------

* neue Codebasis
