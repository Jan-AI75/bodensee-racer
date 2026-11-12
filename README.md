# Bodensee Racer

Arcade-Rennspiel im Stil der 80er (Pseudo-3D): in 5 Etappen einmal rund um den Bodensee, von Lindau bis zurück in den Lindauer Hafen.

**Spielen:** https://jan-ai75.github.io/bodensee-racer/

- Eine einzige `index.html`, Vanilla JS und Canvas 2D, keine Abhängigkeiten
- Für das Handy im Hochformat gemacht, läuft auch am Desktop
- Steuerung: ◀ ▶ und GAS (Touch), Pfeiltasten und Leertaste, optional Neigen des Handys
- Sound synthetisch per Web Audio, abschaltbar

## Einbau in andere Apps

```js
BodenseeRacer.start({
  coins: 3,
  onEnd: (ergebnis) => {
    // { ziel, etappe, km, meter, restzeit, bonus, punkte, neuerRekord, rekord }
  }
});
BodenseeRacer.setCoins(2);
BodenseeRacer.highscore;   // bisheriger Rekord
BodenseeRacer.running;     // läuft gerade eine Runde?
```

Entwicklermodus: `index.html?dev` (Tasten 1–5 springen zur Etappe).
