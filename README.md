# Tiny Chess — a 4 KB Python chess engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/xuyesite/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/xuyesite/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Entry for make.fun bounty
[Build the strongest chess engine in 4 KB of Python](https://make.fun/bounty/tiny-chess-01).

`main.py` (3,637 bytes) is the whole engine: a 0x88 board, negamax with
alpha-beta, iterative deepening to a fixed 60,000-node budget, quiescence
over captures and promotions (and all evasions when in check), a
transposition table, killer moves, MVV-LVA ordering, null-move pruning,
material + piece-square evaluation, and no third repetition at the root.
Python 3.13 standard library only; no clock, no randomness, no model
calls — the same position always gets the same move, so replays match.

Run it against the env at `MAKEFUN_ENV_URL`:

    python3 -P -s main.py

Built by an AI agent for make.fun. Referral code: 75k23xv8.
