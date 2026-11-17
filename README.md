# Guess Who?

A single-page mobile and desktop game. Upload photos of friends and family, crop three levels on each photo (hardest to easiest), then host a guessing game for your friends.

## Features

- Three crop levels per photo, set by you
- Answer choices are the names of everyone in the game (up to 20), in alphabetical order
- Online play: friends join from their own phones with a link or room code (up to 20 players), pick a name, and the first correct answer earns a bonus
- Presenter mode for screen sharing (hides tabs and setup, big photo and answers)
- Players and a scoreboard: tap who answered first, then tap their answer
- Timer per level, game length (10, 20 or endless), results screen
- Groups (Family, Friends, ...) to choose who is in the game
- Skip photo, no repeats until every photo has been shown
- Sound, confetti, keyboard shortcuts, fullscreen, large text and high contrast
- Backup and restore file for all people, crops and settings

Photos stay in the browser on your own device (IndexedDB). Nothing is uploaded anywhere.

## Keyboard shortcuts

Space: next level. Enter: reveal answer. 1-9: pick an answer (on this device). N: next photo. S: skip. P: presenter mode. F: fullscreen. M: sound.

## Online play (join by link)

1. Put the game on GitHub Pages (below). Online play needs the hosted page, not a file opened from disk.
2. On Play, choose Online, then Open lobby. Share your screen so friends can see the photo.
3. Friends open the link (or open the page, tap Join a game and type the 5-letter code) and enter a name. Up to 20 players.
4. Press Start game. Everyone taps a name on their phone. Points: 15 / 10 / 5 by level, plus 5 for the first correct answer.

Notes: connections are peer to peer (PeerJS) and use the free public PeerJS signaling server. Keep the host tab open. Very strict school or office networks can block it. If a phone drops, reopening the link rejoins with the same name.

## Run it

Open `index.html`, or serve the folder:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Host it on GitHub Pages

1. Push these files to a GitHub repository.
2. In the repository, go to Settings, then Pages.
3. Under Build and deployment, choose Deploy from a branch, pick `main` and `/ (root)`, and save.
4. Your game will be at `https://<your-username>.github.io/<repo-name>/`.
