# MrBeast Sudoku Data

**6,840 puzzles** from [onemil.xyz](https://www.onemil.xyz) — clues, solutions, and 4,010 source PDFs.

**Live site:** [delfinadap.github.io/mrbeast-sudoku-data](https://delfinadap.github.io/mrbeast-sudoku-data/)

## Repo structure

```
puzzles.json              ← all 6,840 puzzles (used by the viewer)
puzzles/
  all.json                ← same data, also in puzzles/ for organization
pdfs/
  asktheai/               ← 3,000 PDFs from asktheaiforasudoku.com
  collected/              ← 1,010 PDFs collected from onemil.xyz
```

## Data format

`puzzles.json` — array of objects:

```json
{"i": 100116, "c": "050300007060000008427000530...", "s": "851349627963752148427861539...", "n": 25}
```

| Field | Description |
|-------|-------------|
| `i` | Puzzle ID (from the PDF) |
| `c` | 81-char clue string (0 = blank), left→right, top→bottom |
| `s` | 81-char solution string |
| `n` | Number of given clues |

## Contribute

More data may help crack the transform sequence. Two ways to contribute:

### Option 1: Submit a JSON file
1. Fork this repo
2. Add a JSON file to `puzzles/` (e.g. `puzzles/yourname.json`) — same format as above
3. Open a PR

### Option 2: Submit PDFs
1. Fork this repo
2. Add PDF files to `pdfs/yourname/` (named by puzzle ID, e.g. `123456.pdf`)
3. Open a PR — we'll extract the grids

## Discord

Join us: [discord.gg/KCtjNMJeYv](https://discord.gg/KCtjNMJeYv)
