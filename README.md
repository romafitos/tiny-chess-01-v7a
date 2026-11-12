# Tiny Chess v7a

A four-kilobyte chess engine that fits its whole brain into a single small file.

## How it plays

The program searches with a negamax alpha-beta tree, deepening one layer at a time and calming down quiet lines with quiescence search. A transposition table remembers positions it has already scored, while MVV-LVA captures and killer moves come first in the ordering. The engine also steers away from repeating the same position over and over, and it gives a modest push to pawns that have broken free of every enemy pawn ahead of them.

## Measured strength

Across three graded trials against the house baseline, this version scored 1,326, 1,464 and 1,430, for a mean Elo of 1,407 against the baseline's 1,360.

## Running it

Run it with the system Python and no extra packages:

    python3 -P -s main.py

It only uses the standard library.

## License

MIT.

This entry was built for tiny-chess-01.