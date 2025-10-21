# Wahlhilfe - Anpassung für verschiedene Wahlen

## Dateien anpassen:

### 1. Fragen ändern (`fragen.json`)
- Einfache JSON-Liste mit allen Fragen
- Für jede neue Wahl komplett austauschbar

### 2. Parteipositionen ändern (`parteien.json`)
- Für jede Partei eine Position zu jeder Frage
- Mögliche Werte: `"agree"`, `"neutral"`, `"disagree"`
- Reihenfolge muss mit Fragen übereinstimmen

## Beispiel für neue Partei hinzufügen:
```json
"NEUE_PARTEI": {
  "name": "Neue Partei",
  "positionen": ["agree", "disagree", "neutral", ...]
}
```

## Für neue Stadtratswahl:
1. `fragen.json` mit neuen Fragen überschreiben
2. `parteien.json` mit neuen Parteien/Positionen überschreiben
3. HTML-Datei bleibt unverändert

## Anzahl Fragen/Parteien:
- Beliebig viele Fragen möglich
- Beliebig viele Parteien möglich
- Automatische Sortierung nach Übereinstimmung