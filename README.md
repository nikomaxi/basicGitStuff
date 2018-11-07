This Repository includes all code of Programming 3 group 2

# Some basic git stuff

```sh
$ git status
```
Lists all new or modified files to be committed

```sh
$ git add [file]
```
Snapshots the file in preparation for versioning

```sh
$ git commit -m "[descriptive message]"
```
Records file snapshots permanently in version history

```sh
$ git push
```
Uploads all added files and commits to Git
IMPORTANT: You may have to pull the current branch before pushing new stuff

```sh
$ git pull
```
Downloads bookmark history and incorporates changes

```sh
$ git log
```
Lists version history for the current branch


# Git Branching

### Branch Erstellen
Erstellen einer neuen Branch:
```sh
$ git branch BRANCHNAME
```

Um auf diese Branch zu wechseln benutze:
```sh
$ git checkout BRANCHNAME
```

Dies kann auch Kombiniert werden:
```sh
$ git checkout -b BRANCHNAME
```
Nachdem man auf die Branch gewechselt hat, kann man wie üblich seine Arbeit machen und die Dateien mit 
```sh
$ git add DATEIEN
$ git commit -m "Nachricht"
```
auf Gitlab hochladen.

### Branch auf Gitlab Hochladen

Damit die Branch die du erstellt hast auch für andere des Teams sichtbar ist, muss man die Branch auf Gitlab hochladen
```sh
$ git push -u origin BRANCHNAME
```


### Branch Zusammenführen
Wenn man fertig ist und die Branch mit der Master Zusammenführen möchte, benutzt man:
```sh
$ git checkout master
$ git merge BRANCHNAME
```
Eventuell müssen Dateien zusammengeführt werden die es in der master schon gibt und es zu einem Konflikt kommt. Diese muss man manuell Zusammenführen.

### Branch Löschen
Wenn alles reibungslos Funktioniert hat kann man die gemergte Branch löschen:
```sh
$ git branch -d BRANCHNAME
```
