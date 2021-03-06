# Export für die [Personendatenbank](http://personendatenbank.germania-sacra.de)
Zur Einbindung der Personendaten in die Anzeige der Klosterdatenbank gibt es das Skript [export.php], das den relevanten Teil der Daten als JSON exportiert.

Der Export beinhaltet die relevanten Felder (siehe Liste im Kommentar am Anfang des Skriptes) der Datensätze, die online geschaltet, nicht gelöscht und einem Kloster zugeordnet sind.

Das Skript benötigt die Datei [Aemter.csv](Aemter.csv) mit den Amtsbezeichnungen in Singular und Plural, sowie der Wichtigkeit des Amtes.

Dieses Skript ist auf dem Germania-Sacra Server (mit den richtigen SQL Login Daten) vorhanden. Es kann unter der Adresse http://personendatenbank.germania-sacra.de/export/export.php aufgerufen werden, um den Export zu aktualisieren (Laufzeit Oktober 2013: etwa 15s).

Das Exportergebnis ist danach unter http://personendatenbank.germania-sacra.de/export/export.json verfügbar und wird vom [Indexierungsskript](../klosterdatenbank_neu/#indexierung-der-daten) genutzt.
