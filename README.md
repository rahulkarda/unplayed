# unplayed

**Explore the 10¹²⁰ chess positions humanity has never seen.**

There are more possible chess games than atoms in the observable universe. Humanity has played roughly 10⁹ of them. Every position you reach past move 15 has almost certainly never been seen by human eyes.

*Unplayed* is a browser-based chess explorer that lets you navigate this space — play freely, dive deep, and drop pins on positions worth remembering.

🔗 **[Play it live → unplayed.netlify.app](https://imaginative-biscotti-752260.netlify.app)**

---

## Features

**Exploration**
- Full legal chess engine — castling, en passant, pawn promotion with piece picker
- Territory tracker: Opening → Still in theory → Possibly uncharted → Almost certainly uncharted
- Novelty detection — positions you've never visited before are flagged
- 4 preset positions to jump into (King's Indian, Sicilian, Endgame, Chaos)
- FEN import/export — paste any position from Lichess or Chess.com

**Analysis**
- Position evaluation bar with plain-English label
- Material counter — captured pieces shown above/below board
- Move history with click-to-navigate
- Depth counter and move number

**Computer Opponent**
- Toggle to play against a minimax engine (depth 3, alpha-beta pruning)
- Plays as Black, responds ~120ms after your move

**Discovery**
- Drop a pin on any position — name it, tag it, leave a note
- Your personal atlas persists across sessions (localStorage)
- Load any pinned position back instantly

**Learn**
- 19 chess facts rotating in the ticker — click to advance
- Full Chess Facts panel
- How to Use guide covering every feature

---

## Running locally

No build step. No dependencies. Single HTML file.

```bash
git clone https://github.com/rahulkarda/unplayed
open unplayed/index.html
```

Or just open `index.html` in any browser.

---

## Tech

- Vanilla JS, HTML, CSS — zero dependencies, zero frameworks
- Chess engine written from scratch: legal move generation, castling, en passant, promotion, check/checkmate/stalemate detection, SAN notation with disambiguation
- Minimax with alpha-beta pruning for the computer opponent
- Piece-square tables for position evaluation
- localStorage for pin persistence and novelty tracking

---

## Background

The Shannon number — 10¹²⁰ — is the estimated number of possible chess games. It's named after Claude Shannon, who calculated it in 1950. The number is so large it has no physical analogue. If every atom in the observable universe played a chess game every nanosecond since the Big Bang, you'd still have explored almost none of it.

This project is a meditation on that fact. Every position is a place. Most places have never been visited. The map is yours to make.

---

*Made with no frameworks, one HTML file, and a genuine curiosity about large numbers.*
