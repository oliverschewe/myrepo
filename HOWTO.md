# How-To

## Vorbereitung

Ordner erstellen

```shell
mkdir Uni
cd Uni
```


## Repo clonen
```shell
git clone git@github.com:tyronfranzke/hpi-vorkurs-git.git
```
Ordner `hpi-vorkurs-git` existiert jetzt in Ordner `Uni`.


## neuen Ordner für neues Repo erstellen & Dateien kopieren
Name: `myrepo`
```shell
mkdir myrepo

cp -r hpi-vorkurs-git/* myrepo

// 'cp -r' - um alle Dateien & Unterverzeichnisse zu kopieren
// hpi-vorkurs-git/* - damit keine unsichtbaren Dateien wie Git-Configs aus .git kopiert werden, ansonsten hat man das Repo schon mitkopiert
```
Alle Dateien aus `hpi-vorkurs-git` sind jetzt auch in `myrepo`.

## Überprüfen...
Mit `cd` in den Ordner `repo` gehen und Dateien mit `ls` auflisten
```shell
cd myrepo

ls -l
-------------------
-rw-r--r--  1 oliver.schewe  staff      107  6 Okt 17:45 README.md
-rw-r--r--  1 oliver.schewe  staff  2066082  6 Okt 17:45 memes.pdf
drwxr-xr-x  3 oliver.schewe  staff       96  6 Okt 17:45 mitschriften
drwxr-xr-x  4 oliver.schewe  staff      128  6 Okt 17:45 src
```

## Repo bei Github erstellen
Github-Seite besuchen: [https://github.com/](https://github.com/)

Knöpfe drücken und Daten eingeben...

![](./bilder/1.png)
![](./bilder/3.png)

## Ordner mit dem neuen Repo initialisieren und verknüpfen

siehe Github Befehle im leerem Repo auf Github
![](./bilder/4.png)

Git Repo initialisieren
```git
// Git Repo initialisieren
git init

// Alle Dateien hinzufügen
git add --all

// Commit mit allen Dateien erstellen
git commit -m "first commit"

// Branch "main" erstellen (optional, weil eigentlich Standard)
git branch -M main

// Ordner mit dem Git Repo verlinken
git remote add origin git@github.com:oliverschewe/myrepo.git

// Commit ins Repo pushen
git push -u origin main
```
![](./bilder/5.png)

Github-Repo-Seite im Browser refreshen und freuen (aber nur wenn alle Dateien da sind) ✅

![](./bilder/6.png)

Streicheln...
<center><img src="./bilder/IMG_2017.png" width="600"/></center>