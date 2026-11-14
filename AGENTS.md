# Hinweise für die Rzvation-Hilfe

## Über dieses Projekt

- Hilfeseiten für Rzvation, gebaut mit [Mintlify](https://mintlify.com)
- Seiten sind MDX-Dateien mit YAML-Frontmatter (`title`, `sidebarTitle`, `description`, `keywords`)
- Navigation und Einstellungen stehen in `docs.json`
- Inhalte beschreiben die Anwendung aus dem Repository `muehleis/rzvation`. Bezeichnungen von Menüs, Reitern, Feldern und Schaltflächen werden genau so übernommen, wie sie in der Oberfläche stehen.

## Zielgruppe und Sprache

- Deutsch, Anrede **Sie**
- Einfache Sprache für nicht technisch versierte Leserinnen und Leser: kurze Sätze, ein Gedanke pro Satz, Fachbegriffe erklären
- Tonalität nach der Markenrichtlinie: sachlich, freundlich, präzise – keine Superlative, kein Marketing
- Oberflächenelemente fett: Klicken Sie auf **Speichern**
- Menüwege mit Pfeil: **Organisation → Buchungsseiten**
- Berechtigungsnamen und Dateinamen als Code: `read-reservations`

## Aufbau jeder Seite

1. Ein bis zwei Sätze, worum es geht
2. `<Info>`-Kasten „**Wo finden Sie das?**“ mit Menüweg und – falls möglich – Direktlink
3. Schritt-für-Schritt-Anleitungen mit `<Steps>`, Felder als Tabelle
4. Hinweise mit `<Note>`, `<Tip>`, `<Warning>`
5. `keywords` im Frontmatter pflegen, damit die Suche auch Synonyme findet

Neue Begriffe zusätzlich im **Stichwortverzeichnis** (`stichwortverzeichnis.mdx`) eintragen.

## Terminologie

| Verwenden | Hinweis |
|---|---|
| Objekt | In der Oberfläche heißt es „Objekte“. „Ressource“ nur als Synonym erwähnen. |
| Veranstaltung / Event | Menüpunkt heißt „Events“. |
| Buchung / Reservierung | Beides gleichwertig; Menüpunkt heißt „Reservierungen“. |
| Mitglieder | Bezeichnung ist je Organisation einstellbar (Gäste, Kunden …). |
| Benutzer | Personen mit Zugang zur Verwaltung – nicht mit Mitgliedern verwechseln. |

## Prüfen vor dem Veröffentlichen

```bash
npx mint validate
npx mint broken-links --check-anchors
```

Anker enthalten Umlaute, z. B. `#e-mail-für-benachrichtigungen`.
