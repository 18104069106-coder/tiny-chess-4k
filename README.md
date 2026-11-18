# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/18104069106-coder/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/18104069106-coder/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4,036 bytes of Python: negamax alpha-beta search with a
transposition table, null-move pruning, late-move reductions, check
extensions and a capture quiescence search, over a piece-square-table
evaluation. It searches to a fixed node budget (45,000 nodes a move), never
to a clock, so every game replays move for move. `main.py` is the whole
engine, packed from a readable source with the kit's `makefun compress`.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

Point `MAKEFUN_ENV_URL` at a tiny-chess-01 env (the competition kit's
`program/env/server.mjs`): the engine plays the whole gauntlet, one game
after another, over the env's `/game` and `/move` routes.

---

<sub>Entered on [make.fun](https://make.fun/?ref=0jswgmdt&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
