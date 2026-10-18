# Hi, I'm Zhaoye Wang 👋

High school senior. I build software by directing AI coding tools such as Claude Code: I decide
what to build, test it against real data, and write down what didn't work. The code in these
repos was largely written by those tools, not typed by hand.

## Projects I'd point you to

**[essay-grader](https://github.com/wang2-lat/essay-grader)**: grades AP English Language essays on
the official College Board 6-point analytic rubric and leaves Google-Docs-style margin notes.
- FastAPI + SQLite backend and a Chrome (Manifest V3) extension that grades an open Google Doc from a button on the page.
- Rubric rules (like the Row B grammar cap) are enforced in code, and every margin-note quote is
  checked against the essay text. Notes that don't match are flagged instead of highlighted.
- On 26 held-out official sample essays, total-score agreement is QWK ≈ 0.6. The README
  includes the command to reproduce it and lists known limits.

**[micro-harness](https://github.com/wang2-lat/micro-harness)**: a small, readable agent harness and a
record of benchmarking it.
- The same harness and prompt were run on 7 models over the 2 hardest coding tasks.
- The README documents the iteration from 17% to 50% on hard tasks, including the approaches
  that failed.

**[terminal-arcade](https://github.com/wang2-lat/terminal-arcade)**: terminal games and visualizations
in pure Python `curses` (Snake, Tetris, Minesweeper, Matrix rain, fluid sim, Game of Life …), with a
[GitHub Pages site](https://wang2-lat.github.io/terminal-arcade/).

**[aica](https://github.com/wang2-lat/aica)**: a command-line checker for the EU AI Act's high-risk
requirements (Articles 9–15). It runs offline rule checks with weighted scoring and evidence
validation, and has an optional LLM report. It has 28 tests and runs them in GitHub Actions.

**[native-english-tool](https://github.com/wang2-lat/native-english-tool)**: flags non-native and
"AI-sounding" English (243 word and phrase rules, plus structural checks) and suggests plainer
wording. It has a FastAPI web app, a Chrome extension and 34 tests.

## Common threads

Writing tools (essay-grader, native-english-tool), and checking whether an AI system actually works
(the held-out evaluation in essay-grader, the model benchmarks in micro-harness).
