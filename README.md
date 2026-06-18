# DURARE

Prototipo HTML single-file. Programma di 28 giorni per padri impegnati.

## Cosa c'e

- **`DURARE_app.html`** - versione lite (no backend, no localStorage tracking). Quella da condividere subito. Si apre con doppio click nel browser.
- **`DURARE_app_full_backend-ready.html`** - versione full con gamification (4 indicatori), streak, history, decay. Pronta per essere agganciata a un backend quando lo costruiamo.

## Come provarla

1. Clona il repo (o scarica i due HTML).
2. Apri `DURARE_app.html` in Chrome / Safari / Firefox.
3. Naviga le 4 sezioni dal menu in alto: Home, Programma, Esercizi, Rituali.

## Struttura dell'app

**4 sezioni:**

- **Home** - programma del giorno (selettore D1-D28), pillola psicologica del giorno, mini player musicale integrato, rituale giornaliero suggerito.
- **Programma** - 3 tab: Calendario 28gg cliccabile, Le 4 Fasi, Il Metodo (i 4 pilastri).
- **Esercizi** - 16 esercizi base raggruppati in 4 categorie. Ogni scheda apre il dettaglio con esecuzione, errore comune, varianti e variante "+ figlio".
- **Rituali** - sezione coppia con 3 tab: cosa cambia davvero, rituali quotidiani, rituali del weekend.

## Video Gumlet

Gli esercizi includono video Gumlet hostati nel workspace Gumlet di Emanuele. 19 video totali integrati. Asset ID nel JavaScript di ciascun HTML (cerca `videoSolo` / `videoFiglio` nel `const ESERCIZI = [...]`).

## Music player

Il mini player nella home legge file MP3 dalla cartella `./audio/` accanto all'HTML (path `./audio/track-01.mp3` ... `track-10.mp3`). I file vanno scaricati separatamente da Pixabay o simili (vedi cartella audio nel repo del prodotto).

## Tecnologie

- HTML5 + CSS3 + JS vanilla, single file
- Nessuna dipendenza npm, nessun build
- Font: Fraunces + Inter + JetBrains Mono (Google Fonts CDN)
- Audio: HTML5 `<audio>` con file locali
- Video: iframe Gumlet
- Storage (solo full): localStorage

## Versione

v5.2 - giugno 2026. Lite + full duplicati per evoluzione futura.

