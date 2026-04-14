# Better Wordle

Your Wordle companion — narrow down the answer faster with smart filtering and strategic guess suggestions.

## How to Use

### 1. Enter Known Positions (Green & Yellow Letters)

The five letter inputs correspond to positions 1–5 of the Wordle grid.

- **Green letter (exact match):** Type the letter and keep the **Exact** checkbox checked.
- **Yellow letter (right letter, wrong position):** Type the letter and **uncheck** the Exact checkbox. The letter is automatically added to the "Contains" filter — no need to re-enter it.

### 2. Contains (Yellow Letters)

Letters that must appear somewhere in the word. Yellow letters from the position inputs are added here automatically, but you can also type additional letters manually.

### 3. Excludes (Gray Letters)

Letters confirmed not to be in the word. Type all gray letters here.

> **Tip:** If the same letter appears as both yellow and gray (e.g., a word has one "E" but not two), enter it in both Contains and Excludes. The solver handles this correctly — Contains takes priority, so valid words won't be eliminated.

### 4. Read the Results

- **Possible Words** — Ranked by letter frequency so the most likely answers appear first.
- **Words to Try** — Strategically chosen guesses that test the most untested letters still common among remaining candidates. Use these to maximize information per guess.

## Features

- **Auto yellow-to-contains** — Yellow position letters are automatically treated as "must contain."
- **Frequency-ranked results** — Possible words are scored by how common their letters are in the remaining pool.
- **Strategic suggestions** — "Words to Try" are picked to reveal the most new information.
- **Overlap handling** — Correctly handles letters that are both yellow and gray (duplicate letter scenarios).
- **Starter word** — A random word suggestion to kick off your game.

## Example Workflow

1. Guess **CRANE** in Wordle.
2. Result: **C** gray, **R** yellow (pos 2), **A** green (pos 3), **N** gray, **E** yellow (pos 5).
3. In Better Wordle:
   - Position 2: type `R`, uncheck Exact.
   - Position 3: type `A`, keep Exact checked.
   - Position 5: type `E`, uncheck Exact.
   - Excludes: type `cn`.
4. Review **Possible Words** for likely answers and **Words to Try** for your next strategic guess.
