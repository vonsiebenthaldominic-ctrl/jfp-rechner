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

1. Datei in `dist/` anpassen. Preise, Kategorien und Angebote stehen oben in `rechner.js` im Block `KONFIGURATION` (`categories`, `packages`, `extraHourPrice`, `kmPrice` usw.)
2. Committen
3. Neues Release mit nächster Version erstellen, z. B. `v1.0.1`
4. Im Webflow-Embed die Versionsnummer anpassen (`@1.0.0` → `@1.0.1`) und publishen

Rollback: im Embed einfach wieder die vorherige Version eintragen.

## Versionen

- `1.0.0` – Erstversion
- `1.0.1` – CSS-Korrekturen (Formular, PDF-Bereich)
- `1.1.0` – Kategorien (Hochzeit & Verlobung, Shootings, Business & Event); Zusatzstunde CHF 450; Zweitfotograf entfernt; CHF 0.65/km
- `1.2.0` – Überschriften und Fliesstexte nutzen Webflow-Klassen (`classes` in der Konfiguration)
- `1.3.0` – Kleinere Überschriften: Hauptüberschriften `h4-heading`, Unterüberschriften und Kachelnamen `h5-heading`
- `1.4.0` – Bewerbungsfotos entfernt; «Euer Richtpreis» über dem Ergebnis entfernt; keine Kursivschrift mehr (Website und PDF)
