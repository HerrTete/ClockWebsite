# ClockWebsite

Eine einfache Webseite, die die aktuelle Uhrzeit oder einen Countdown anzeigt.

## Varianten & Beispiele

### 1. Einfache Uhrzeit

Ohne URL-Parameter wird die aktuelle Uhrzeit angezeigt.

```
https://clock.herrtete.de
```

### 2. Countdown bis zu einer Uhrzeit (heute)

Mit dem Parameter `time` (Format `HH:MM` oder `HH:MM:SS`) wird ein Countdown bis zur angegebenen Uhrzeit am heutigen Tag angezeigt.

```
https://clock.herrtete.de?time=18:00
https://clock.herrtete.de?time=18:00:00
```

### 3. Countdown bis zu einem bestimmten Datum und einer Uhrzeit

Mit dem zusätzlichen Parameter `date` (Format `TT.MM.JJJJ`) wird bis zu einem konkreten Datum und einer Uhrzeit heruntergezählt.

```
https://clock.herrtete.de?date=31.12.2026&time=00:00:00
```

### 4. Countdown mit Titel

Mit dem optionalen Parameter `title` wird eine Beschriftung oberhalb des Countdowns angezeigt. Ohne `title` wird standardmäßig „Countdown" angezeigt.

```
https://clock.herrtete.de?date=31.12.2026&time=00:00:00&title=Silvester
```

## URL-Parameter Übersicht

| Parameter | Format          | Beschreibung                                      |
|-----------|-----------------|---------------------------------------------------|
| `time`    | `HH:MM[:SS]`    | Zieluhrzeit; aktiviert den Countdown-Modus        |
| `date`    | `TT.MM.JJJJ`   | Zieldatum (optional, Standard: heute)             |
| `title`   | beliebiger Text | Titel über dem Countdown (optional, Standard: „Countdown") |