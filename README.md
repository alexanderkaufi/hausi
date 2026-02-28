# Webseite auf GitHub veröffentlichen

Diese Seite ist als statische Webseite vorbereitet (`index.html`).

## 1) Einmalig auf deinem Mac ausführen (Git freischalten)

Auf deinem Rechner ist Git aktuell durch die Xcode-Lizenz blockiert.

```bash
sudo xcodebuild -license
```

Lizenz bis zum Ende durchgehen und mit `agree` bestätigen.

## 2) Neues Repository auf GitHub erstellen

1. Auf GitHub auf **New repository** klicken.
2. Namen wählen, z. B. `hausi-kontrolling`.
3. **Public** auswählen.
4. Repository erstellen (ohne README, wenn du dieses lokale Projekt direkt hochladen willst).

## 3) Projekt hochladen

```bash
cd "/Users/alkaufimacbook/SynologyDrive/Informatik/Codex Projekte/Hausi Kontrolling"
git init
git add .
git commit -m "Initial website"
git branch -M main
git remote add origin https://github.com/DEIN-USERNAME/DEIN-REPO.git
git push -u origin main
```

## 4) GitHub Pages aktivieren

1. Repository auf GitHub öffnen.
2. **Settings** -> **Pages**.
3. Unter **Build and deployment**:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` und `/ (root)`
4. Speichern.

Danach ist die Seite erreichbar unter:

- `https://DEIN-USERNAME.github.io/DEIN-REPO/`

Wenn das Repo `DEIN-USERNAME.github.io` heißt, dann direkt:

- `https://DEIN-USERNAME.github.io/`
