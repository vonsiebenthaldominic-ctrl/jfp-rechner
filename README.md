# Richtpreis-Rechner – Jordan Fuss Photography

Hochzeits-Konfigurator für die Webflow-Website, ausgeliefert über jsDelivr.

## Dateien

- `dist/rechner.js` – Logik, Preise, Pakete, Logo für das PDF
- `dist/rechner.css` – Styles (alle Klassen mit Präfix `jfo-`)
- `webflow-embed.html` – Snippet für das Code-Embed-Element in Webflow

Der Google-API-Key liegt bewusst **nicht** im Repo, sondern nur im Webflow-Embed.

## Einbindung in Webflow

Inhalt von `webflow-embed.html` in ein **Code Embed**-Element kopieren.
Das Webflow-Formular für die Anfrage braucht die ID `jfo-anfrage`.

## Update-Ablauf

1. Datei in `dist/` anpassen (z. B. Preise in `rechner.js`, Bereich `packages` bzw. `extraHourPrice` usw.)
2. Committen
3. Neues Release mit nächster Version erstellen, z. B. `v1.0.1`
4. Im Webflow-Embed die Versionsnummer anpassen (`@1.0.0` → `@1.0.1`) und publishen

Rollback: im Embed einfach wieder die vorherige Version eintragen.

## Versionen

- `1.0.0` – Erstversion
