# cheat_sheet_jh
## Filesystem Display & Navigation

code | englisch | deutsch
--- | --- | ---
*.* | the current direcotry | Das aktuelle Verzeichnis ist gemeint
*q* | Exit command | Exit Befehl
*Befehl + --help* | Display command usage information including available flags and proper syntax | Anzeige von Informationen zur Befehlsverwendung, einschließlich verfügbarer Flags und korrekter Syntax
*man + Befehl* | Display the manual page of specified command | Zeigt das Manual für angegebenen Befehl an
*whatis + Befehl* | Display a one line brief summary of specified command | Zeigt eine einzeilige Zusammenfassung des angegebenen Befehls an
*pwd*|Show the present working directory | Zeigt das aktuelle Verzeichnis an
*ls*|List all the files in a directory | Listet alle Dateien in einem Verzeichnis auf
*ls -l*|List all files and their details (owner, mtime, size, etc) | Listet alle Dateien dateillierter auf (Eigentümer, Mtime, Größe usw.)
*ls -a*|List all the files in a directory (including hidden files) | Listet alle Dateien in einem Verzeichnis auf (einschließlich versteckter Dateien)
*ls -la* | List all files and hidden files and their details| Alle Dateien, auch versteckte Dateinen, werden detalliert angezeigt
*file*|View the type of any file | Zeigt den Typ einer beliebigen Datei an
*du -sh* | Shows the size of the current directory| Zeigt die Größe des aktuellen Verzeichnisses an
*diff -qr Pfad1 Pfad2* | Compare contents of two folders | Inhalte von zwei Ordnern vergleichen
*rsync*|Synchronize the changes of one directory to another | Änderungen eines Verzeichnisses mit einem anderen Verzeichnis synchronisieren
*diskutil list* |List all disks and partitions| Alle Plsatten und Partitionen anzeien
*find . -type f -name '\.*' -print * | Find Dot Files | Zeigt Punkdateien Hiddenfiles an
*cd*|Change directory to some other location | Zu einem anderen Verzeichnis wechseln
*cd ..*|Change directory one level up | Eine Verzeichnisebene nach oben wechseln
*cd -*|Change directory to the last path | Zum letzten Arbeitspfad wechseln
*sudo reboot* | Reboot system | System neu starten
*sudo halt* | Shutdown system| System herunterfahren
---

## File Manipulation

code | english | deutsch
--- | --- | --- |
*mkdir*|Create a new directory| Neuen Ordner erstellen
*touch*|Create a new, empty file, or update the modified time of an existing one| Neue Datei erstellen (Dateinamen + Dateiendung mit angeben Bsp.: touch style.css)
*cp -a* | Copy with all rights | Kopiert mit allen Rechten
*cp <Dateiname_alt.txt> <Dateiname_neu.txt>* | Copy file with a given name | Eine Datei wird mit entsprechenden Namen dupliziert und kopiert
*mv -rvf* | Move or rename file or directory | Verschieben oder Umbenennen von Dateien und Ordnern
*mv <Dateiname_alt.txt> <Dateiname_neu.txt>* | Rename File | Dateiname ändern, aber wenn es den Dateinamen schon gibt, wird die Datei überschrieben
*mv -i* | Name change with advance warning | Namensänderung mit Vorwarnung
*mv <dateiname.txt> Ordnername* | Move file to folder| Datei in Ordner verschieben 
*rm* | Delete file | Datei löschen
*rm -rf* Ordnername| Delete folder | Ordner löschen
*chmod -R 777* | Change the file permissions for a file or directory | Vergibt für User, Gruppe & Anderen für alle Unterverzeichnisse read, write, execute Rechte
*chmod 777 Verzeichnispfad*| Change the file permission for a special folder |Vergibt für User, Gruppe & Anderen für einen speziellen Ordner read, write, execute Rechte
*cat > file* | Create a new file with the text you type after | Neue Datei mit Text erstellen
*cat file*|View the contents of a file| Inhalt einer Datei anzeigen
*greb*|View the contents of a file that match a pattern | Zeigen Sie den Inhalt einer Datei an, die einem Muster entspricht

***
***

## Markdown

### Heading
```no-highlight (Codebloecke werden entweder mit 3 Backticks am Anfang und am Ende dargestellt oder mit 4 Leerzeichen vor der Raute. Das Verwenden der drei Backticks wird empfohlen. Zudem ist es nicht noetig, nach den Backticks Text zu schreiben, es dient nur der Vereinfachung und Darstellung.)
# H1
## H2
### H3
#### H4
##### H5
###### H6

Alternativ fuer H1 und H2

Alt-H1
======

Alt-H2
------
```

Beispiele

# H1
## H2
### H3
#### H4
##### H5
###### H6

Alternativ fuer H1 und H2

Alt-H1
======

Alt-H2
------

***

### Emphasis


```Codeblock Hervorhebungen

Italic mit *Sternchen* oder _Unterstrichen_

Bold mit zwei **Sternchen** oder __Unterstrichen__

Italic und Bold kombiniert **_Sternchen_** und **_Unterstrichen_**
oder auch so
**_Sternchen_ und _Unterstrichen_**
oder so
**Sternchen und _Unterstrichen_**

Durchgestrichen mit zwei ~~Tilden~~

Farbig hervorgehoben mit zwei ==Gleichzeichen==
```

Beispiele
Italic mit *Sternchen* oder _Unterstrichen_

Bold mit zwei **Sternchen** oder zwei __Unterstrichen__

Italic und Bold kombiniert **_Sternchen_** und **_Unterstrichen_**
oder auch so
**_Sternchen_ und _Unterstrichen_**
oder so
**Sternchen und _Unterstrichen_**

Durchgestrichen mit zwei ~~Tilden~~

Farbig hervorgehoben mit zwei ==Gleichzeichen==

***

### Horizontal Rule

Absätze werden dargetsellt mit 3 oder mehr

```
***
Sternchen

---
Bindestriche

___
Unterstriche
```

Beispiele

***
Sternchen

---
Bindestriche

___
Unterstriche



Line Breaks
--
Hier startet der Text.

Ich füge nun einen Absatz mit zwei Zeilenumbrüchen ein (zweimal Enter).


Dies ist auch ein eigener Absatz. 
Mit Trennung durch einen Zeilenumbruch, ist der zweite Satz im Absatz separiert, gehört aber dennoch zu diesem.
****

### Lists

```Codeblock für Listen
Ordered List (Geordnete Liste)
1. Erstes Element
2. Zweites Element
3. Drittes Element
  1. Erstes Element einer geordneten Unterliste

Unordered List (Ungeordnete Liste)
- Erstes Element
- Zweites Element
- Drittes Element
    - Erstes Element einer ungeordneten Unterliste

Aufzählungsstriche können mit Plus +, Sternchen * oder Bindestrichen - aufgeführt werden    
````
Ordered List
1. Erstes Element
2. Zweites Element
3. Drittes Element
    1. Erstes Element einer geordneten Unterliste


Unordered List
- Erstes Element
- Zweites Element
- Drittes Element
    - Erstes Element einer ungeordneten Unterliste

***

### Tables
```
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

Die äußeren Striche sind nicht nötig, siehe unten:
Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
```

Beispiel

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |



Die äußeren Striche sind nicht nötig, siehe unten:
Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
***

### Code and Syntax
```
Inline `code` hat Backticks vorne und hinten.
````
Inline `code` hat Backticks vorne und hinten.

Codebloecke werden entweder mit 3 Backticks am Anfang und am Ende dargestellt oder mit 4 Leerzeichen vor der Raute. Das Verwenden der drei Backticks wird empfohlen. Zudem ist es nicht noetig, nach den Backticks Text zu schreiben, es dient nur der Vereinfachung und Darstellung.


```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

javascript
var s = "JavaScript syntax highlighting";
alert(s);


***
### Links

```Codeblock für Links
Einfachste Weise einen Link einzufügen
[Titel des Links] Link
[Google](https://www.google.de/)

Man kann Links auch so darstellen
[link text itself], oder so
https://www.google.de/ oder so
<https://www.google.de/>
````
Einfachste Weise einen Link einzufügen:
[Google](https://www.google.de/)

Man kann Links auch so darstellen
[google.de], oder so
https://www.google.de/ oder so
<https://www.google.de/>

***

Images

````
Google Logo:

![alt text] (https://www.google.de/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)
````

Google Logo

![alt text](https://www.google.de/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)

***