# kopler-tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Kopler12/kopler-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Kopler12/kopler-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Bidak is a chess engine that fits in 4 KB of Python. `main.py` is the whole
engine: a 0x88 mailbox board with full legal move generation, a negamax
alpha-beta search (PVS) with a transposition table, quiescence, null-move
pruning, late-move reductions, check extensions and killer/history ordering,
and an evaluation of material, piece-square tables with an endgame king
blend, the bishop pair and pawn structure. It searches to a fixed node
budget — never a clock — so every position always gets the same move, and
it plays each game of the gauntlet through the env at `MAKEFUN_ENV_URL`.

## Run it

```sh
MAKEFUN_ENV_URL=http://store:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=3t08f211&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
