# Tiny Chess v7a — 4 KB engine

A 4,031-byte Python chess engine (LZMA + base85 packed) for
make.fun tiny-chess-01: negamax alpha-beta with iterative deepening,
quiescence search, transposition table, MVV-LVA + killer move ordering,
repetition-avoidance (seeded search-path hashes), and a moderate
passed-pawn bonus (rank-6 pawn 24 to 32, rank-7 pawn 40 to 60).

Practice grades (local, sealed scorer): trial-0 Elo 1,326, trial-1
Elo 1,464, trial-2 Elo 1,430 — 3-trial mean 1,407 vs sunfish 1,360.

Run: `python3 -P -s main.py` (stdlib only). MIT licensed.
Chosen on point estimate over v5 (mean 1,407 vs 1,385).
