# 60

Ein minimalistisches Browser-Reflexspiel: Klicke so viele Punkte wie möglich in 60 Sekunden.

Ein einzelner runder Punkt erscheint an einer zufälligen Position auf einem weißen Bildschirm. Jeder Treffer gibt +1 Punkt, der Punkt verschwindet mit einer kurzen Pop-Animation und taucht sofort an neuer Stelle wieder auf. Ein Zeitbalken oben zeigt die verbleibende Rundenzeit; in den letzten 10 Sekunden wechseln Timer und Balken auf Rot. Dein Highscore wird lokal im Browser gespeichert.

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

## Tech-Stack

- Reines Vanilla JavaScript, HTML und CSS — kein Framework, kein Build-Tool, keine externen Abhängigkeiten
- Alles in einer `index.html` (HTML, CSS und JS inline)
- Highscore-Persistenz über `localStorage`
- Läuft direkt über GitHub Pages, da `index.html` im Repo-Root liegt

## Lizenz

[MIT](LICENSE)
