# tiny-chess-01

A 4 KB Python chess engine for the make.fun tiny-chess-01 bounty.

The engine uses iterative-deepening alpha-beta search with a fixed 100,000-node cap per move, counted cumulatively and checked in both the main search and quiescence, so no move can run away on time. It also uses quiescence search, a transposition table, a Zobrist repetition check from the game history, and a material plus piece-square-table evaluation. It is deterministic: fixed node budget, no clock, no unseeded randomness.

The entrypoint `main.py` is produced from the readable `engine.py` with the kit's `makefun compress` command.

Practice trials (local kit harness): Elo 1191 / 1099 / 1364, average 1218, with zero timeouts. Slowest move 5.34 s against a 10 s move limit.

MIT license.
