# Mac & iOS Shortcuts Learning Game ⌨️

An interactive browser-based trainer for mastering Mac and iOS keyboard shortcuts, with spaced repetition so the more you nail a shortcut, the less often it shows up.

## Features

- **130+ shortcuts** across 9 categories: Mac General, Screenshots, Finder, System, Text Editing, Browser, iOS hardware keyboard, iPadOS Globe key, and Accessibility
- **Spaced repetition** — shortcuts you get wrong come back more often; ones you've mastered fade into the background
- **Category picker** — drill all shortcuts or focus on a specific category
- **Quick Drill** (10 questions) and **Extended Drill** (30 questions)
- **Two question types** — identify the shortcut from a description, or identify what a shortcut does
- **Score tracking** — per-shortcut accuracy, overall stats, streak, and mastery count
- **Full reference** — searchable list of all shortcuts, browsable by category
- Progress is saved automatically in your browser (localStorage)

## How to Use

Just open `shortcuts_game.html` in any modern browser — no install, no dependencies, no server needed.

```
open shortcuts_game.html
```

### Menu options

| Option | Description |
|---|---|
| ⚡ Quick Drill | 10 questions, ~2 minutes |
| 🔥 Extended Drill | 30 questions, ~6 minutes |
| 📊 My Scores | Per-shortcut progress with mastery indicators |
| 📖 All Shortcuts | Searchable full reference |

## Shortcut Categories

| Category | Count |
|---|---|
| Mac • General | 38 |
| Mac • Screenshots | 7 |
| Mac • Finder | 27 |
| Mac • System | 10 |
| Mac • Text Editing | 19 |
| Mac • Browser | 15 |
| iOS • Hardware Keyboard | 20 |
| iPadOS • Globe Key | 9 |
| Mac • Accessibility | 7 |

## How Spaced Repetition Works

Each shortcut has a weight that starts at 10. A correct answer lowers the weight (min 1); a wrong answer raises it (max 25). Questions are selected randomly but weighted, so weaker shortcuts appear proportionally more often. There's no fixed schedule — just keep drilling and the system adapts.

## Tech

Single self-contained HTML file. Vanilla JS, no frameworks, no build step. All state is stored in `localStorage` under the key `shortcuts_trainer_v2`.
