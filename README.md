# cheat_sheet_jh
## File System Display and Navigation

code | englisch | deutsch
--- | --- | ---
*pwd*|Show the present working directory | Zeigt das aktuelle Arbeitsverzeichnis an
*ls*|List all the files in a directory | Alle Dateien in einem Verzeichnis auflisten
*ls -l*|List all files and their details (owner, mtime, size, etc) | Alle Dateien und ihre Details auflisten (Eigentümer, Mtime, Größe usw.)
*ls -a*|List all the files in a directory (including hidden files) | Alle Dateien in einem Verzeichnis auflisten (einschließlich versteckter Dateien)
*file*|View the type of any file | Zeigen Sie den Typ einer beliebigen Datei an
*nano file*|Open a file (or create new one) in nano text editor | Öffnen Sie eine Datei (oder erstellen Sie eine neue) im Nano-Texteditor
*vim file*|Open a file (or create new one) in vim text editor| Öffnen Sie eine Datei (oder erstellen Sie eine neue) im vim-Texteditor
*rsync*|Synchronize the changes of one directory to another | Synchronisieren Sie die Änderungen eines Verzeichnisses mit einem anderen
*du -sh* | Shows the size of the current directory| Zeigt die Groeße des Verzeichnisses an, in dem man sich befindet
*find . -type f -name '\.*' -print * | Find Dot Files | Zeigt Punkdateien an
*cd*|Change directory to some other location | Zu einem anderen Verzeichnis wechseln
*cd ..*|Change directory one level up | Eine Verzeichnisebene nach oben wechseln
*cd -*|Change directory to the last path | Zum letzten Arbeitspfad wechseln

## File Manipulation

code | english | deutsch
--- | --- | --- |
*mkdir*|Create a new directory| Neuen Ordner erstellen
*touch*|Create a new, empty file, or update the modified time of an existing one| Neue Datei erstellen (Dateinamen + Dateiendung mit angeben)
*cp -a* | Copy with all rights | Kopiert mit allen Rechten
*cp <Dateiname_alt.txt> <Dateiname_neu.txt>* | | Eine Datei wird mit entsprechenden Namen dupliziert und kopiert
*mv -rvf* | Move or rename file or directory | Verschieben oder Umbenennen von Dateien und Ordnern
*mv <Dateiname_alt.txt> <Dateiname_neu.txt>* | Rename File | Dateiname ändern, aber wenn es den Dateinamen schon gibt, wird die Datei überschrieben
*mv -i* | Name change with advance warning | Namensaenderung mit Vorwarnung
*mv <dateiname_alt.txt> <Ordnername>* | | Datei in Ordner verschieben 
*rm* | delete file | Datei loeschen
*rm -rf* | delete folder | Ordner loeschen
*chmod -R 777* | Change the file permissions for a file or directory | Rechte fuer Ordner und Dateien ändern
*cat > file* | Create a new file with the text you type after | Neue Datei mit Text erstellen
*cat file*|View the contents of a file| Inhalt einer Datei anzeigen
*greb*|View the contents of a file that match a pattern | Zeigen Sie den Inhalt einer Datei an, die einem Muster entspricht

## Markdown

Element | Markdown Syntax
---|---|
Heading | 