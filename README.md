# Tiny Chess — a 4 KB chess engine in Python

[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![make.fun rank](https://make.fun/badge/tiny-chess-01/fulede9394/makefun-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![make.fun reward](https://make.fun/badge/tiny-chess-01/fulede9394/makefun-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01)

An original chess engine in a single `main.py` (at most 4,096 bytes) for the
[make.fun](https://make.fun) tiny-chess-01 bounty: the strongest chess engine
in 4 KB of Python. It plays the house gauntlet through the env — 8 games,
one against each rung from depth-2 up to nodes-2M.

Engine: 0x88 board, full legal move generation (castling, en passant,
promotion), alpha-beta with iterative deepening to a fixed node budget
(never a clock, so trials replay byte for byte), quiescence over captures,
promotions and check replies, transposition table, killer-move ordering,
MVV-LVA capture ordering, and an evaluation of material + piece-square
tables + bishop pair.

## Try make.fun

https://make.fun/r/5kkq1ant
