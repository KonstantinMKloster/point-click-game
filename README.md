# 60

Minimalistische Browser-Minispiele: jede Runde dauert 60 Sekunden.

**🎯 Punkte klicken** — Ein einzelner runder Punkt erscheint an einer zufälligen Position auf einem weißen Bildschirm. Jeder Treffer gibt +1 Punkt, der Punkt verschwindet mit einer kurzen Pop-Animation und taucht sofort an neuer Stelle wieder auf.

**⌨️ Text tippen** — Ein Text läuft wie bei einem Teleprompter von unten ins Bild und verblasst nach oben hin. Richtig getippte Buchstaben färben sich schwarz, falsche rot; mit Backspace lässt sich korrigieren. Bei jeder Runde wird eine neue, zufällige Textreihenfolge zusammengestellt.

Beide Spiele zeigen einen ablaufenden Zeitbalken oben, der in den letzten 10 Sekunden auf Rot wechselt, und speichern den Highscore lokal im Browser. „Text tippen" benötigt eine physische Tastatur.

## Play now

▶️ [Jetzt spielen](https://KonstantinMKloster.github.io/point-click-game/)

*(Link aktiv, sobald GitHub Pages für dieses Repo aktiviert ist: Settings → Pages → Deploy from branch → `main` / root.)*

## Lokal spielen

Kein Build-Step nötig — einfach `index.html` im Browser öffnen:

```bash
git clone https://github.com/KonstantinMKloster/point-click-game.git
cd point-click-game
open index.html   # macOS
# oder die Datei direkt per Doppelklick öffnen
```

## Struktur

- `index.html` – Spielauswahl (Menü) mit Highscore-Übersicht
- `dot.html` – Spiel „Punkte klicken"
- `type.html` – Spiel „Text tippen"

Jede Seite ist vollständig eigenständig (HTML, CSS und JS jeweils inline, kein gemeinsamer Build-Step nötig).

## Tech-Stack

- Reines Vanilla JavaScript, HTML und CSS — kein Framework, kein Build-Tool, keine externen Abhängigkeiten
- Highscore-Persistenz über `localStorage` (`dotgame_highscore`, `typegame_highscore_words`)
- Läuft direkt über GitHub Pages, da `index.html` im Repo-Root liegt

## Lizenz

[MIT](LICENSE)
