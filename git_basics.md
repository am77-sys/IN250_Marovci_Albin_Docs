# Git Basics – Dokumentation (IN250)

## Aufgabe 1: Repository auf GitHub erstellen
Ich habe auf GitHub ein neues Git Repository mit dem Namen
IN250_Marovci_Albin_Docs erstellt.
Das Repository wurde leer erstellt, ohne README oder weitere Dateien.

## Aufgabe 2: Repository klonen
Anschliessend habe ich das Repository mit dem Befehl
`git clone` auf meinen lokalen Linux-Rechner geklont.
Danach bin ich in den Projektordner gewechselt und habe den Status geprüft, in dem ich den Command 'git status' eingegeben habe.


## Aufgabe 2: Repository klonen
Ich habe das zuvor erstellte GitHub-Repository mit dem Befehl
`git clone` auf meinen lokalen Rechner geklont und danach in
den Projektordner gewechselt.

## Aufgabe 3: Markdown Cheatsheet und Initial Commit
Ich habe mein zuvor erstelltes Markdown Cheatsheet in den Ordner
des geklonten Git-Repositories kopiert.
Anschliessend habe ich die Datei zum Repository hinzugefügt und
einen Commit mit der Nachricht "Initial commit" erstellt.

## Aufgabe 4: .gitignore erstellen
Ich habe eine .gitignore-Datei erstellt, um bestimmte Dateien dauerhaft vom Repository auszuschliessen.
Eingetragen habe ich:
- *.log
- GeheimeBankInformationen.txt

Danach habe ich die Datei committed ("Add gitignore") und auf GitHub gepusht.

## Aufgabe 5: Zweites lokales Repository (git init)
Ich habe in einem neuen Ordner ein lokales Repository mit `git init` erstellt.
Danach habe ich das bestehende GitHub-Repository als Remote `origin` hinzugefügt.
Mit `git pull origin main` habe ich den aktuellen Stand vom Remote heruntergeladen.

Beobachtung:
Mehrere lokale Repositories können mit demselben Remote verbunden sein.
Nach einem Pull sind die Dateien im neuen Ordner identisch zum Remote-Stand.
Wenn ich im alten Ordner vorher gepusht habe, sind diese Änderungen im neuen Ordner nach dem Pull sichtbar.
Beobachtung:
Beim Erstellen eines neuen lokalen Repositories mit `git init`
wurde standardmässig der Branch `master` verwendet.
Das bestehende GitHub-Repository nutzte jedoch den Branch `main`.

Beim Pushen aus dem neuen Repository wurde deshalb ein zusätzlicher
Branch `master` im Remote Repository erstellt.
Git führt Branches nicht automatisch zusammen.


## Aufgabe 6: Warum Git und warum zuerst Commit und Push?

Git wird in der Softwareentwicklung eingesetzt, um Änderungen an Dateien
nachvollziehbar zu versionieren. Es ermöglicht mehreren Personen gleichzeitig
am selben Projekt zu arbeiten, Änderungen zu vergleichen und bei Fehlern
auf frühere Versionen zurückzugehen. Dadurch wird die Zusammenarbeit
strukturierter und sicherer.

Im Fall eines Feuers sollte man zuerst einen `git commit` und danach einen
`git push` ausführen, weil ein Commit die Änderungen lokal speichert und ein
Push diese zusätzlich im Remote Repository sichert. Selbst wenn der lokale
Rechner danach beschädigt wird, sind die Änderungen im Remote Repository
weiterhin verfügbar.
