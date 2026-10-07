# Global Insights – GitHub Pages

Diese Version ist als statische GitHub-Pages-Webseite vorbereitet.

## Enthalten
- `index.html` – komplette Dashboard-Datei
- Interaktive Weltkarte mit MapLibre/OpenFreeMap und automatischem Offline-Fallback
- 165 eingebettete Kernstädte
- zusätzlicher Welt-Städtekatalog: Die HTML-Datei versucht beim Online-Laden einen GeoNames-basierten Katalog mit 5.979 Städten ab 100.000 Einwohnern einzubinden
- Nachrichten, Weltweite Politik, Wissenschaft, Analysen, Metropolen, Landkreise und Sicherheitsbereich
- responsive Oberfläche für Desktop, iPad und Android
- Flight-Radar-Funktion ist nicht enthalten

## GitHub Pages veröffentlichen
1. Auf GitHub ein neues Repository erstellen.
2. `index.html` in das Hauptverzeichnis (`/`) des Repositorys hochladen.
3. Optional `README-GITHUB.md` mit hochladen.
4. Repository öffnen → **Settings** → **Pages**.
5. Bei **Build and deployment**: **Deploy from a branch** auswählen.
6. Branch `main` und Ordner `/ (root)` auswählen.
7. **Save** drücken.
8. Nach dem Deployment erscheint die GitHub-Pages-Adresse in den Pages-Einstellungen.

## Wichtig für die Karte und den erweiterten Städtekatalog
Die Karte und der erweiterte Weltkatalog nutzen externe, öffentlich erreichbare Dienste. GitHub Pages selbst hostet die HTML-Datei, aber diese externen Daten werden im Browser geladen. Falls ein Dienst nicht erreichbar ist, fällt die Karte auf eine integrierte Offline-Karte zurück; der eingebettete Kernkatalog bleibt verfügbar.

## Vor dem produktiven Einsatz
Die im Dashboard enthaltenen Nachrichten, Kurse, Ereignisse und sonstigen Daten sind teilweise statisch bzw. als Demo-/Recherchebestand eingebettet. Für ein dauerhaft automatisch aktualisiertes Live-System sollten anschließend echte Datenquellen/APIs mit Quellen, Zeitstempeln und Fehlerbehandlung angebunden werden.
