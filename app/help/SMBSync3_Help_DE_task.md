### Testmodus

Es wird kein Überschreiben und Löschen der Datei durchgeführt, wenn Sie dies prüfen. Testen Sie bitte, wenn Sie eine Synchronisationsaufgabe erstellen, Dateien, die kopiert oder gelöscht werden, finden Sie in der Registerkarte Nachricht.

### Automatische Synchronisierungsaufgabe

Wenn dieses Kontrollkästchen aktiviert ist, wird die Aufgabe auf die automatische. Aufgaben, die auf automatische Synchronisierung eingestellt sind, werden gestartet, wenn Sie die Synchronisierungstaste drücken.

### Aufgabenname

Geben Sie den Aufgabennamen an.

### Sync-Typ

Die Sync-Methode wird aus Spiegeln, Kopieren, Verschieben, Archivieren ausgewählt. Die Synchronisierung erfolgt vom Master zum Ziel in eine Richtung.

- Spiegeln
- Verschieben
- Kopieren
- Archivieren

### Tauschen von Quelle und Ziel

Tauschen Sie den Inhalt des Quellordners und des Zielordners 

### Quellordner

Tippen Sie auf die Schaltfläche, um den Quellordner zu bearbeiten

### Zielordner

Tippen Sie auf die Schaltfläche, um den Zielordner zu bearbeiten

### Dateien für die Synchronisierung auswählen

Wenn Sie kein Häkchen setzen und dann alle Dateien synchronisieren. Wenn Sie ein Häkchen setzen, um Details zu sehen. 

- Audiodateien synchronisieren  
  Wenn Sie ein Häkchen setzen, um die Dateien mit den folgenden Erweiterungen zu synchronisieren.  
  aac, aif, aifc, aiff, kar, flac, m3u, m4a, mid, midi, mp2, mp3, mpga, ogg, ra, ram, wav  
- Bilddateien synchronisieren  
  Wenn Sie ankreuzen, die Dateien mit den folgenden Erweiterungen zu synchronisieren.  
  bmp, cgm, djv, djvu, gif, ico, ief, jpe, jpeg, jpg, pbm, pgm, png, tif, tiff
- Videodateien synchronisieren  
  Wenn Sie ankreuzen, dass Sie die Dateien mit den folgenden Erweiterungen synchronisieren möchten.  
  avi, m4u, mov, mp4, movie, mpe, mpeg, mpg, mxu, qt, wmv  
- Dateifilter  
  Sie können den Namen und die Erweiterung der Datei, die Sie synchronisieren möchten, mit anderen als den oben genannten auswählen.

### Unterverzeichnisse für die Synchronisierung auswählen

Wenn Sie das Kontrollkästchen nicht aktivieren, werden alle Unterverzeichnisse synchronisiert. Wenn Sie das Häkchen setzen, wird die Schaltfläche Verzeichnisfilter angezeigt.

- Verzeichnisfilter
  Sie können den Namen des Verzeichnisses auswählen, das Sie synchronisieren möchten.

### Sync-Aufgabe nur beim Laden ausführen

Wenn diese Option aktiviert ist, können Sie die Synchronisierung nur während des Ladevorgangs starten. Wenn die Synchronisierung gestartet wird, während nicht geladen wird, führt dies zu einem Fehler.

### Bestätigen Sie, bevor Sie das Kopieren oder Löschen außer Kraft setzen

Es wird ein Bestätigungsdialog angezeigt, wenn Sie die Datei überschreiben und löschen wollen, wenn Sie das Häkchen gesetzt haben.

### Fehleroptionen  

Sie können das Verhalten beim Auftreten eines Fehlers festlegen.

- Synchronisation stoppen
- Alle Fehler ignorieren und nachfolgende Aufgaben starten
  Verwenden Sie diese Option, wenn Sie sicherstellen möchten, dass nachfolgende Aufgaben ausgeführt werden. 
- Folgeaufgaben starten, wenn Netzwerkoptionen zu Fehlern führen  
  Verwenden Sie diese Option, wenn Sie nachfolgende Aufgaben ausführen möchten, wenn die Adresse nicht privat ist oder wenn es sich nicht um die angegebene IP-Adresse handelt.  

### Netzwerk

- Auch im ausgeschalteten Zustand ausführen  
  Sie können immer die Synchronisierung starten
- Conn mit einem beliebigen AP  
  Die Synchronisierung kann starten, wenn das drahtlose LAN mit einem beliebigen Zugangspunkt verbunden ist.
- Hat eine private Adresse  
  Sie können die Synchronisierung starten, wenn die IP-Adresse eine private Adresse ist
- IP-Adressliste  
  Sie können die Synchronisierung nur starten, wenn die WiFi-IP-Adresse mit einer der angegebenen Adressen übereinstimmt. Sie können auch die aktuelle IP-Adresse, mit der Ihr Gerät verbunden ist, direkt über die IP-Auswahlliste hinzufügen.  
  Sie können Wildcards für den Filter verwenden. (z. B.: 192.168.100.\*, 192.168.\*.\*.)

### Zeigt erweiterte Optionen

**Bitte verwenden Sie es, wenn Sie detaillierte Optionen einstellen.**

### Unterverzeichnisse einbeziehen

Es werden rekursiv Unterverzeichnisse unter dem angegebenen Hauptordner einbezogen. 

### Leere Verzeichnisse einbeziehen

Synchronisiert die leeren Verzeichnisse (auch wenn ein Verzeichnis auf dem Master leer ist, wird es auf dem Ziel erstellt). Wenn nicht markiert, werden leere Verzeichnisse auf dem Master ignoriert. 

### Versteckte Verzeichnisse einbeziehen

Wenn diese Option aktiviert ist, schließt Sync die versteckten Linux-Verzeichnisse ein (diejenigen, deren Name mit einem Punkt beginnt). Beachten Sie, dass in Windows und Samba das Attribut "versteckt" nicht durch den Ordnernamen gesetzt wird. Daher hat der synchronisierte Ordner auf dem SMB/Windows-Ziel nicht das Attribut "versteckt" des Hosts. 

### Versteckte Dateien einschließen

Wenn diese Option aktiviert ist, schließt Sync die versteckten Linux-Dateien ein (diejenigen, deren Name mit einem Punkt beginnt). Beachten Sie, dass unter Windows und Samba das Attribut "versteckt" nicht durch den Dateinamen gesetzt wird. Daher hat die synchronisierte Datei auf dem SMB/Windows-Ziel nicht das Attribut "versteckt" des Hosts.

### Zieldateien überschreiben

Wenn diese Option nicht aktiviert ist, werden die Dateien auf dem Ziel niemals überschrieben, auch wenn die Vergleichskriterien nach Größe und Zeit unterschiedlich sind. 

### Wiederholung bei Netzwerkfehler (nur für SMB-Freigaben)

Bei serverseitigen Verbindungsfehlern wird SMBSync3 die Synchronisation maximal 3 Mal im Abstand von 30 Sekunden erneut versuchen. 

### SMB I/O-Schreibpuffer auf 16KB begrenzen (nur für SMB-Freigaben)

**Bitte versuchen Sie es, wenn Sie beim Schreiben in den PC/NAS-Ordner die Fehlermeldung "Access is denied" erhalten.

Wenn diese Option aktiviert ist, wird der I/O-Puffer für Schreibvorgänge auf dem SMB-Host auf 16 KB begrenzt. 

### Dateien vor der Synchronisierung löschen (nur im Spiegelmodus)

Wenn dieses Kontrollkästchen aktiviert ist, werden zuerst die Verzeichnisse und Dateien gelöscht, die im Zielordner vorhanden sind, aber nicht auf dem Master existieren. Danach werden die Dateien und Ordner, die anders sind, auf das Ziel kopiert.

Wenn es sich bei dem Masterordner um einen SMB-Ordner handelt, verlängert sich die Verarbeitungszeit, da die Verzeichnisstruktur und deren Inhalt über das Netzwerk gescannt wird. Es wird dringend empfohlen, die Option " SMB2-Verhandlung verwenden" zu aktivieren, da SMB1 sehr langsam ist.

### Verzeichnisse und Dateien entfernen, die von den Filtern ausgeschlossen wurden

Wenn diese Option aktiviert ist, **entfernt sie Verzeichnisse/Dateien, die von den Filtern ausgeschlossen sind**. 

### Letzte Änderungszeit der Zieldatei nicht auf die Quelldatei setzen

Bitte aktivieren Sie diese Option, wenn Sie eine Fehlermeldung erhalten wie SmbFile#setLastModified()/File#setLastModified() schlägt fehl. Das bedeutet, dass der Remote-Host das Setzen der letzten Änderungszeit der Datei nicht zulässt. Wenn diese Option nicht aktiviert ist, wird die letzte Änderungszeit der kopierten Datei auf dem Ziel auf den Zeitpunkt des Kopierens/Synchronisierens gesetzt. Das bedeutet, dass die Zieldatei neuer erscheint als die Masterdatei. 

Für die nächsten Synchronisationen können Sie:

- dabei bleiben, nur nach Größe zu vergleichen, oder

- Sie können die Option "Zieldatei nicht überschreiben, wenn sie neuer als die Quelldatei ist" aktivieren, um nur Dateien zu kopieren, die später auf dem Master geändert wurden, oder

- Sie können die Task-Option "Letzte Änderungszeit von Dateien aus der benutzerdefinierten Liste der SMBSync3-Anwendung abrufen" aktivieren. Diese Option ist jedoch derzeit nicht verfügbar, wenn das Ziel SMB ist. Die meisten SMB-Hosts unterstützen die Einstellung der letzten Änderungszeit. 

Im Folgenden finden Sie detaillierte Informationen zu den einzelnen Optionen. 

### Dateigröße verwenden, um festzustellen, ob Dateien unterschiedlich sind

Wenn diese Option aktiviert ist, werden Dateien als unterschiedlich betrachtet, wenn sie sich in der Größe unterscheiden. 

### Nur Größe vergleichen

Dateien werden nur dann als unterschiedlich betrachtet, wenn die Größe der Quelle größer ist als die des Ziels. Damit wird der Vergleich nach Dateizeit deaktiviert. 

### Zeit der letzten Änderung verwenden, um festzustellen, ob Dateien unterschiedlich sind 

Wenn diese Option aktiviert ist, werden Dateien anhand des Zeitpunkts der letzten Änderung als unterschiedlich betrachtet 

### Minimal zulässiger Zeitunterschied (in Sekunden) zwischen Quell- und Zieldatei

Dateien werden als identisch betrachtet, wenn der Unterschied zwischen ihren letzten Änderungszeiten kleiner oder gleich der gewählten Zeit in Sekunden ist. Sie gelten als unterschiedlich, wenn die Zeitdifferenz zwischen den Dateien größer als die gewählte Zeit ist. FAT und ExFAT benötigen eine Mindesttoleranz von 2 Sekunden. Wenn 0 Sekunden gewählt wird, müssen die Dateien genau die gleiche Zeit haben, um als ähnlich zu gelten.

### Zieldatei nicht überschreiben, wenn sie neuer ist als die Quelldatei

Wenn diese Option aktiviert ist, wird die Datei nur dann überschrieben, wenn die Stammdatei neuer ist als die Zieldatei, auch wenn die Dateigrößen und die letzten Aktualisierungszeiten unterschiedlich sind. Beachten Sie, dass bei einem Wechsel der Zeitzone oder bei einer Änderung der Dateien während der Zeitspanne der Sommerzeitumstellung die zuletzt geänderte Datei älter erscheinen kann als die nicht aktualisierte Datei. Dies hängt mit den Unterschieden im Dateisystem zusammen, und nur eine manuelle Überprüfung vor dem Überschreiben der Datei kann Datenverluste vermeiden. Es wird allgemein empfohlen, Dateien während des Intervalls der Sommerzeitumstellung nicht zu ändern, wenn sie automatisch synchronisiert werden sollen 

### Tageslicht-Sparzeit-Differenz zwischen Dateien ignorieren

Hier können Sie den Zeitunterschied in Minuten zwischen Sommer- und Winterzeit einstellen. Dateien werden als unterschiedlich betrachtet, wenn die Zeitdifferenz nicht genau dem angegebenen Intervall entspricht (+/- der in der vorherigen Option angegebenen "Min. erlaubten Zeitdifferenz (in Sekunden)")

### Verzeichnis- und Dateinamen überspringen, die ungültige Zeichen enthalten(", :, \, *, <, >, |)

Wenn diese Option aktiviert ist, wird eine Warnmeldung angezeigt und die Synchronisierung wird fortgesetzt, ohne die Verzeichnisse/Dateien zu verarbeiten, die ungültige Zeichen enthalten. 

### Löschen des Masterverzeichnisses, wenn es leer ist (nur wenn die Sync-Option Verschieben ist)

Wenn der Sync-Modus Verschieben ist, wird nach dem Verschieben der Dateien auf das Ziel auch der Master-Ordner gelöscht. 

### Wenn das Datum und die Uhrzeit nicht über die EXIF-Daten ermittelt werden können, wird eine Bestätigungsmeldung angezeigt

Anzeige einer Bestätigungsmeldung, wenn das übernommene Datum und die Uhrzeit nicht aus den Exif-Daten ermittelt werden können.

### Quelldateien, die größer als 4 GB sind, bei der Synchronisation auf einen externen Speicher ignorieren.

Wenn dieses Kontrollkästchen aktiviert ist, können Sie E/A-Fehler bei der Synchronisierung mit einer MicroSD-Karte vermeiden, indem Quelldateien, die größer als 4 GB sind, bei der Synchronisierung mit dem lokalen Speicher ignoriert werden.

### Ignoriere Dateien, deren Dateiname 255 Bytes überschreitet

Wenn diese Option aktiviert ist, werden Dateien mit Dateinamen, die länger als 255 Byte sind, ignoriert.