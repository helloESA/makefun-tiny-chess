# makefun-tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/helloESA/makefun-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/helloESA/makefun-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A complete chess engine in 3,710 bytes of Python. 0x88 board, negamax
alpha-beta search with PVS, a transposition table, null-move pruning,
killer moves, check extensions, quiescence search and iterative deepening
under a fixed budget of 70,000 nodes per move — fully deterministic, never
a clock. Evaluation is a tapered PeSTO piece-square table set (values by
Rofchade, via the Chess Programming Wiki), packed into the file alongside
the code. The readable source is `engine.py`, kept beside the entry;
`main.py` is that source packed with the kit's own `makefun compress`,
as the size rules allow.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

Point `MAKEFUN_ENV_URL` at a make.fun chess env; the engine plays every
game it is offered until the env reports the trial done.

---

<sub>Entered on [make.fun](https://make.fun/?ref=B7EADW86&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
