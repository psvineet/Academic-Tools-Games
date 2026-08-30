# Academic Tools & Games

A single-page hub of small, self-contained academic tools and browser games. Each item is a standalone `index.html` — no build step, no dependencies, just open and use.

**Live hub:** `index.html` at the repo root — expandable category cards linking straight to each tool/game.

## Structure

```
.
├── index.html                          # main navigator / landing page
├── tools/
│   ├── chemistry/
│   │   └── ccc/                        # Chemical Concentration Calculator
│   ├── health/
│   │   ├── bmi/                        # BMI Calculator
│   │   └── dsc/                        # Dose Calculator
│   ├── math/
│   │   ├── calculator/                 # Scientific Calculator
│   │   └── pc/                         # Scientific Prefix Converter
│   ├── misc/
│   │   └── rg/                         # Resume Generator
│   ├── pharma-academic/
│   │   └── pcsg/                       # Patient Case Summary Generator
│   └── utilities/
│       └── uc/                         # Universal Unit Converter
└── games/
    ├── Color Match/
    ├── Memory Match/
    ├── Number Puzzle/
    ├── Quick Math Quiz/
    ├── Tic Tac Toe/
    └── Word Unscramble Master/
```

Every tool/game folder contains a single `index.html` that runs entirely client-side (HTML, CSS, and JS inline — no external build artifacts).

## Categories

| Category | Tools |
|---|---|
| Chemistry | Chemical Concentration Calculator |
| Health | BMI Calculator, Dose Calculator |
| Math | Scientific Calculator, Scientific Prefix Converter |
| Misc | Resume Generator |
| Pharma Academic | Patient Case Summary Generator |
| Utilities | Universal Unit Converter |
| Games | Color Match, Memory Match, Number Puzzle, Quick Math Quiz, Tic Tac Toe, Word Unscramble Master |

## Running locally

No server or install required:

```bash
git clone https://github.com/psvineet/Academic-Tools-Games.git
cd Academic-Tools-Games
open index.html        # macOS
# or
xdg-open index.html    # Linux
# or just double-click index.html in a file browser
```

Each tool/game also works standalone — you can open its `index.html` directly without going through the hub.

## Adding a new tool or game

1. Create a new folder under `tools/<category>/<short-name>/` (or `games/<Game Name>/` for a game) containing an `index.html`.
2. Add a matching entry card in the root `index.html` under the right category section, linking to the new folder.
3. Keep each page self-contained (inline CSS/JS) so it can be opened independently of the hub.

## Notes

- The hub UI uses Google Fonts (Noto Sans) loaded via CDN — an internet connection is needed for fonts to render correctly, though the tools themselves work offline.
- Folder and file names are kept stable since the hub links to them by path — renaming a tool folder requires updating its link in `index.html`.

## Contact

Maintained by VPS — connect.vps@icloud.com
