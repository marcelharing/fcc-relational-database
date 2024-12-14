### Git Cheatsheet

#### Repository erstellen und initialisieren
- **`git init`**: Initialisiert ein neues Git-Repository im aktuellen Verzeichnis.
- **`git clone <repository-url>`**: Klont ein bestehendes Repository von einer URL.

#### Änderungen verfolgen
- **`git status`**: Zeigt den aktuellen Status des Repositories an (untracked, staged, modified).
- **`git add <datei>`**: Fügt eine Datei zur Staging-Area hinzu.
- **`git add .`**: Fügt alle Änderungen im aktuellen Verzeichnis zur Staging-Area hinzu.
- **`git commit -m "<Nachricht>"`**: Erstellt einen Commit mit einer Nachricht.

#### Branches verwalten
- **`git branch`**: Listet alle lokalen Branches auf.
- **`git branch <branch-name>`**: Erstellt einen neuen Branch.
- **`git checkout <branch-name>`**: Wechselt zu einem anderen Branch.
- **`git checkout -b <branch-name>`**: Erstellt einen neuen Branch und wechselt zu ihm.
- **`git branch -d <branch-name>`**: Löscht einen Branch.

#### Remote-Repositories verwalten
- **`git remote -v`**: Listet alle Remote-Repositories auf.
- **`git remote add <name> <url>`**: Fügt ein neues Remote-Repository hinzu.
- **`git remote remove <name>`**: Entfernt ein Remote-Repository.
- **`git push <remote> <branch>`**: Überträgt lokale Commits zu einem Remote-Repository und den entsprechenden Remote Branch.
- **`git pull <remote> <branch>`**: Holt Änderungen von einem Remote-Repository und integriert sie in den aktuellen Branch.

#### Änderungen anzeigen
- **`git log`**: Zeigt die Commit-Historie an.
- **`git diff`**: Zeigt die Unterschiede zwischen den Änderungen an.
- **`git show <commit>`**: Zeigt die Änderungen eines bestimmten Commits an.

#### Änderungen zurücksetzen
- **`git reset <datei>`**: Entfernt eine Datei aus der Staging-Area.
- **`git reset --hard`**: Setzt alle Änderungen im Arbeitsverzeichnis und in der Staging-Area zurück (Achtung: Alle uncommitteten Änderungen gehen verloren).
- **`git revert <commit>`**: Erstellt einen neuen Commit, der die Änderungen eines bestimmten Commits rückgängig macht.

#### Konfiguration
- **`git config --global user.name "<dein-name>"`**: Setzt den Benutzernamen für Git.
- **`git config --global user.email "<deine-email>"`**: Setzt die E-Mail-Adresse für Git.
- **`git config --global --list`**: Listet alle globalen Konfigurationseinstellungen auf.

### Sonstiges
- **`git fetch`**: Holt Änderungen von einem Remote-Repository, ohne sie in den Arbeitsbereich zu integrieren.
- **`git merge`**: Integriert die Änderungen in den Arbeitsbereich. `git fetch` und `git merge` machen zusammen das selbe wie git pull 

## Schnellablauf:
`git init` <br>
`git add .`<br>
`git commit -m "meine Änderung"`<br>
`git add remote add origin https://github.com/benutzername/repository-name.git`<br>
`git push -u origin main` - oder --set-upstream verknüpft lokalen branch main mit remote branch origin/main. Dann ist keine Angabe von branch oder remote mehr notwendig.
