# tiny-chess-01

A 4 KB Python chess engine for the make.fun tiny-chess-01 bounty.

- Iterative-deepening alpha-beta search with a fixed 100,000-node cap per move (checked in search and quiescence), so no move can time out.
- Quiescence search, transposition table, piece-square-table evaluation.
- Deterministic: fixed node budget, no clock, no randomness.

Practice trials (kit, local): Elo 1191 / 1099 / 1364, average 1218, zero timeouts. Max move 5.34 s (limit 10 s).

MIT license.
