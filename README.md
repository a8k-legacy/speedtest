# SpeedTest Game

A unique typing speed test that evaluates capability based on difficulty and word count rather than WPM. This project marked my first substantial use of TypeScript and involved solving complex logic and algorithmic challenges.

**Game Concept**: The test does not depend on Words Per Minute (WPM). Instead, it assesses capability by presenting words according to the selected difficulty and number of words (max 30 per game). Success depends on typing accuracy within strict time limits per word.

## Technical Architecture

### Core Components

- **Game Engine**: Real-time word matching algorithm
- **State Management**: Pure TypeScript implementation with type-safe transitions
- **DOM Manipulation**: Optimized batch updates
- **Persistence Layer**: LocalStorage for theme preferences

### Key Features

- 4 Difficulty Levels (Easy, Normal, Hard, Insane)
- Adaptive Time Limits (JSON-configurable)
- Input Validation System with anti-cheat mechanisms
- Theme System (Light/Dark) with CSS Variables
- Sound Feedback System

### Difficulty Levels Explained

- **Easy**: Simple words with 5 seconds per word. Max wrongs: number of words × 0.5
- **Normal**: Medium-difficulty words with 4 seconds per word. Max wrongs: number of words × 0.25
- **Hard**: Hard and long words with 4 seconds per word. Max wrongs: 1
- **Insane**: Words as hard as 'Hard' difficulty but with only 2 seconds per word. Max wrongs: 1

## How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/a8k-legacy/speedtest.git
   cd speedtest
   ```

2. **Install dependencies and compile TypeScript** (requires TypeScript installed globally):
   ```bash
   npm install -g typescript
   tsc --project tsconfig.json
   ```

3. **Open `index.html` in a browser** or use a static server like `live-server`.

## Codebase Structure

```
speedtest/
├── audio/                  # Sound files
├── Images/                 # Theme assets
├── src/                    # TypeScript source (Main.ts)
├── dist/                   # Compiled JS
├── index.html              # Main entry point
├── style.css               # Styles
├── words.json              # Word database
└── tsconfig.json           # TypeScript configuration
```

## Enhanced Version

A restyled and enhanced version of this game is featured in the [a8k-games-hub](https://games.a8k.dev).

---

*Part of the A8K Legacy archive—a collection of early projects and learning experiments by [Saif Abdelrazek](https://saifabdelrazek.com).*
