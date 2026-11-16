# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/leitmotiv34/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/leitmotiv34/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 3,731 bytes of Python (main.py, lzma-packed). 0x88 board,
alpha-beta search with a transposition table, principal-variation search,
late-move reductions, quiescence and check evasions under a fixed
60,000-node budget per move; material plus piece-square evaluation with an
endgame king table. Fully deterministic: no clock, no randomness, the same
position always gets the same move. It plays the make.fun tiny-chess-01
gauntlet through the contest env over HTTP.

## Run it

```sh
MAKEFUN_ENV_URL=<contest env url> python3 main.py
```

It plays every game the env serves, one after another, and exits when the
env reports the trial done.

---
<sub>Entered on [make.fun](https://make.fun/?ref=0jtgc9vt&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
