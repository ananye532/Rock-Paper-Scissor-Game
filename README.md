# Rock Scissors Paper

A minimal, single-file browser game built with vanilla HTML, CSS, and JavaScript.

## Preview

```
✊  vs  🖐️
you lose!
Wins: 3  Draws: 1  Losses: 2
```

## Getting Started

No install. No dependencies. No build step.

```bash
# Just open the file in any browser
open index.html
```

## How to Play

1. Click ✊ Rock, ✌️ Scissors, or 🖐️ Paper
2. CPU picks randomly
3. Result and score update instantly

**Win conditions**
- Rock beats Scissors
- Scissors beats Paper
- Paper beats Rock

## Project Structure

```
index.html   ← entire game lives here
README.md
```

## How It Works

The entire game logic is one object and one function.

```js
const beats = { rock: 'scissors', scissors: 'paper', paper: 'rock' };

function play(you) {
  const cpu = moves[Math.floor(Math.random() * 3)];
  if (you === cpu)         // draw
  else if (beats[you] === cpu)  // win
  else                     // lose
}
```

`beats[you] === cpu` is the only win condition check needed. No switch statements, no chained if-else.

## Tech Stack

| Layer | Choice |
|---|---|
| Markup | HTML5 |
| Styling | Vanilla CSS |
| Logic | Vanilla JS |
| Dependencies | None |

## License

MIT — do whatever you want with it.
