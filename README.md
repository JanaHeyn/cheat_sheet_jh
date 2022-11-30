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
*ls -l*|List all files and their details (owner, mtime, size, etc) | Listet alle Dateien dateillierter auf (Rechte, Eigentümer, Mtime, Größe usw.)
*ls -a*|List all the files in a directory (including hidden files) | Listet alle Dateien in einem Verzeichnis auf (einschließlich versteckter Dateien)
*ls -la* | List all files and hidden files and their details| Alle Dateien, auch versteckte Dateinen, werden detalliert angezeigt
*ls -R* | Displays the contents of the current folder and its subfolders | Zeigt den Inhalt des aktuallen Ordners und dessen Unterordner an
*file*|View the type of any file | Zeigt den Typ einer beliebigen Datei an
*du -sh* | Shows the size of the current directory| Zeigt die Größe des aktuellen Verzeichnisses an
*diff -qr Pfad1 Pfad2* | Compare contents of two folders | Inhalte von zwei Ordnern vergleichen
*rsync*|Synchronize the changes of one directory to another | Änderungen eines Verzeichnisses mit einem anderen Verzeichnis synchronisieren
*diskutil list* |List all disks and partitions| Alle Plsatten und Partitionen anzeien
*find . -type f -name '\.*' -print * | Find Dot Files | Zeigt Punkdateien Hiddenfiles an
*cd* oder *cd ~* | Change to the home directory | Ins Homeverzeichnis wechseln
*c Doppeltab* | What options are available in the current folder for movement (display of the order) | Welche Möglichlkeiten im aktuellen Ordner zur Bewegung vorhanden sind (Darstellung der Order)
*cd /:* | Root directory | Root Verzeichnis
*cd .. oder cd ./..*|Change directory one level up | Eine Verzeichnisebene nach oben wechseln
*cd ./../../* | Change directory two levels up | geht zwei Ordnerebenen nach oben
*cd ./../Ordnername* | Opens a specific folder one level above the current folder (Gewschister folder) | Öffnet einen spezifischen Ordner eine Ebene über dem aktuellen Ordner (Gewschisterordner)
*cd ./Ordnername1/Ordnername2* | Opens a specific folder, within another specific folder above it. | Öffnet einen spezifischen Ordner, innerhalb eines anderen darüberliegenden spezifsichen Ordners   
*cd -*|Change directory to the last path | Zum letzten Arbeitspfad wechseln

*sudo reboot* | Reboot system | System neu starten
*sudo halt* | Shutdown system| System herunterfahren
***

## File Manipulation

code | english | deutsch
--- | --- | --- |
*mkdir*|Create a new directory| Neuen Ordner erstellen
*touch*|Create a new, empty file, or update the modified time of an existing one| Neue Datei erstellen (Dateinamen + Dateiendung mit angeben Bsp.: touch style.css)
*cp -a* | Copy with all rights | Kopiert mit allen Rechten
*cp <Dateiname_alt.txt> <Dateiname_neu.txt>* | Copy file with a given name | Eine Datei wird mit entsprechenden Namen dupliziert und kopiert
*mv -rvf* | Move or rename file or directory | Verschieben oder Umbenennen von Dateien und Ordnern
*mv <Dateiname_alt.txt> <Dateiname_neu.txt>* | Rename File | Dateiname ändern (bewegt den Inhalt einer Datei in eine neue Datei)
*mv -i* | Name change with advance warning | Namensänderung mit Vorwarnung
*mv <dateiname.txt> Ordnername* | Move file to folder| Datei in Ordner verschieben 
*rm* | Delete file | Datei löschen
*rmdir* | Delete folder (only if it is empty) | Löscht einen Ordner (nur wenn er leer ist)
*rm -rf* Ordnername| Delete folder with all contents | Ordner löschen mit allen Inhalten
*chmod -R 777* | Change the file permissions for a file or directory | Vergibt für User, Gruppe & Anderen für alle Unterverzeichnisse read, write, execute Rechte
*chmod 777 Verzeichnispfad*| Change the file permission for a special folder |Vergibt für User, Gruppe & Anderen für einen speziellen Ordner read, write, execute Rechte
*cat > Dateiname* | Create a new file with the text you type after | Neue Datei mit Text erstellen
*cat Dateiname*|View the contents of a file in the terminal| Inhalt einer Datei wird im Terminal angezeigt
*cat Dateiname1 Dateiname2 > Dateiname3* | Merges 2 files and their contents into a new file | Fügt 2 Dateien und deren Inhalt zu einer neuen Datei zusammen
*greb*|View the contents of a file that match a pattern | Zeigen Sie den Inhalt einer Datei an, die einem Muster entspricht
***

## Git & Github
### Git Kommandozeile

code | english | deutsch
--- | --- | ---
*git clone* | Copy a repo from Github locally | Ein Repo von Github lokal kopieren
*git add .* | Add changes | Änderungen hinzufügen
*git commit -m "Place commit here"* | Add comment what was changed | Kommentar hinzufügen, was gemacht wurde
*git push* | Copy the file to github | Kopiert die Datei wieder auf Github
*git status* | Displays the status | Gibt den Status aus
*git log* | List of all activities | Auflistung aller Aktivitäten
*echo + text* | | Gibt einen Befehl im Terminal aus
*echo "text" >> Dateiname | | Speichert einen Text in der angegebenen Datei  

***

### Git commits 
Die Commits werden immer auf Englisch geschrieben und mit einem der folgenden Wörter (großgeschrieben) begonnen. Commits sollen eher kurz gehalten werden, durchaus ist es möglich auf die genaue Position oder den spezifischen Namen hinzuweisen.
- Create
- Add
- Change
- Fix
- Delete

Wenn ein "Issue" bearbeitet wird damit ein Problem behoben wird, dann wird auf das entsprechende Issue referenziert. 
Dies wird wie folgt dargestellt:
- Strat mit dem Wort Fix
- Raute #
- Semikolon ;
- Commit Nachricht

```
Beispiel:
- "Fix #1; Add commit-rules.md file"
- "Fix #877; Change installation instructions in README.md file"
```

##### Privates Repo zu einer Orga hinzufügen
> Ein privates Repo kann mit "Fork" in eine gewünschte Orga umkopiert werden. 

> Änderungen werden nicht in beiden Repos automatisch gleichzeitig übernommen und müssten dann entsprechend hinzugefügt werden.

##### Ein neues Repo im Temrinal erstellen

````
echo "# bla" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:JanaHeyn/bla.git
git push -u origin main
````

##### Ein bestehendes Repo auf Github "pushen"

```
git remote add origin git@github.com:JanaHeyn/bla.git
git branch -M main
git push -u origin main
```


***
***
***

## Markdown

### Header
```
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

Darstellung:

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
```
Italic/Kursiv mit *Sternchen* oder _Unterstrichen_

Bold/Fett mit zwei **Sternchen** oder __Unterstrichen__

Italic und Bold kombiniert **_Sternchen_** und **_Unterstrichen_**
oder auch so
**_Sternchen_ und _Unterstrichen_**
oder so
**Sternchen und _Unterstrichen_**

Durchgestrichen mit zwei ~~Tilden~~

Farbig hervorgehoben mit zwei ==Gleichzeichen==
```

Darstellung:
Italic/Kursiv mit *Sternchen* oder _Unterstrichen_

Bold/Fett mit zwei **Sternchen** oder zwei __Unterstrichen__

Italic und Bold kombiniert **_Sternchen_** und **_Unterstrichen_**
oder auch so
**_Sternchen_ und _Unterstrichen_**
oder so
**Sternchen und _Unterstrichen_**

Durchgestrichen mit zwei ~~Tilden~~

Farbig hervorgehoben mit zwei ==Gleichzeichen==
***

### Trennlinien
```
Absätze werden wie folgt dargstellt mit 3 oder mehr

***
Sternchen

---
Bindestriche

___
Unterstriche
```

Darstellung:
***
Sternchen

---
Bindestriche

___
Unterstriche
***

### Line Breaks
Hier startet der Text.

Ich füge nun einen Absatz mit zwei Zeilenumbrüchen ein (zweimal Enter).


Dies ist auch ein eigener Absatz. 
Mit Trennung durch einen Zeilenumbruch, ist der zweite Satz im Absatz separiert, gehört aber dennoch zu diesem.
****

### Listen
```
Ordered List (sortierte Liste)
1. Erstes Element
2. Zweites Element
3. Drittes Element
  1. Erstes Element einer geordneten Unterliste

Unordered List (unsortierte Liste)
- Erstes Element
- Zweites Element
- Drittes Element
    - Erstes Element einer ungeordneten Unterliste

Aufzählungsstriche können mit Plus +, Sternchen * oder Bindestrichen - aufgeführt werden    
````
Darstellung:
Ordered List (sortierte Liste)
1. Erstes Element
2. Zweites Element
3. Drittes Element
    1. Erstes Element einer geordneten Unterliste

Unordered List (unsortierte Liste)
- Erstes Element
- Zweites Element
- Drittes Element
    - Erstes Element einer ungeordneten Unterliste
***

### Aufgabenliste

````
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
````

Darstellung
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
***

### Zitate
````
Zitate können mit einem Rechtspfeil > eingefügt werden.
````
> Zitat 1

> eingerückter Zitat 2
***

### Tabellen
```
| Spalte 1                | Spalte 2        | Spalte 3                 |
|:------------------------|:---------------:|-------------------------:|
| Spalte 1 links zentriert| Spalte 2 centred| Spalte 3 rechts zentriert|

Mit einem Doppelpunkt rechts, links oder an beiden Seite innerhalb der Trennlinien wird die Ausrichtung des Textes bestimmt.

Die äußeren Striche sind nicht nötig, siehe unten:

so      | gehts   | auch
--------|---------|-----
*Still* |`renders`| **nicely**
1       | 2       | 3

```

Darstellung:

| Spalte 1                | Spalte 2        | Spalte 3                 |
|:------------------------|:---------------:|-------------------------:|
| Spalte 1 links zentriert| Spalte 2 centred| Spalte 3 rechts zentriert|

Mit einem Doppelpunkt rechts, links oder an beiden Seite innerhalb der Trennlinien wird die Ausrichtung des Textes bestimmt.

Die äußeren Striche sind nicht nötig, siehe unten:

so      | gehts   | auch
--------|---------|-----
*Still* |`renders`| **nicely**
1       | 2       | 3
***

### Code und Syntax
```
Inline `code` oder auch eine Zeile Code hat je einen Backtick vorne und hinten.
````
Darstellung:
Inline `code` oder auch eine Zeile Code hat je einen Backtick vorne und hinten.

```
Codebloecke bzw mehrere Zeilen Code, werden mit 3 Backticks am Anfang und am Ende des Paragraphs dargestellt.
Wenn nach den Backticks die Progarmmiersparche steht, dann wird es automatisch erkannt und farblich hinterlegt.
```

Nach den Backticks nichts angegeben:
```
console.log("Hallo Welt");
alert("Hello");
```

Programmiersprache nach den Backticks angegeben (js):
```js
console.log("Hallo Welt");
alert("Hello");
```
***

### Links

```Codeblock für Links
Einfachste Weise einen Link einzufügen:
Titel des Link ins eckigen Klammern + Link in runden Klammern
[Google](https://www.google.de/)

Alternativ
Sobald man mit der Maus über den Link hovert, wird Name angezeigt
[Titel des Links] Link "Name"
[Google](https://www.google.de/ "Name")

Man kann Links auch so darstellen
[link text itself], oder so
https://www.google.de/ oder so
<https://www.google.de/>
````
Darstellung:
Einfachste Weise einen Link einzufügen:
[Google](https://www.google.de/)

Alternativ
Sobald man mit der Maus über den Link hovert, wird Name, in dem Fall Google, angezeigt.
[Google](https://www.google.de/ "Google")

Man kann Links auch so darstellen
[google.de], oder so
https://www.google.de/ oder so
<https://www.google.de/>
***

### Bilder
```
Funktioniert ähnlich wie beim Link, davor wird ein Ausrufezeichen gesetzt gefolgt von eonem Akternativtext, falls das Bild nciht angeziegt werden kann.
Google Logo

![Dies ist das Logo von Google](https://www.google.de/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)
```
Darstellung:
Google Logo

![Dies ist das Logo von Google](https://www.google.de/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)
***
