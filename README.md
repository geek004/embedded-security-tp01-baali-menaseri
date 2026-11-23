# TP 01 – Operation Ghost Bus (CAN bus)

University of Batna 2 – CESE ING 5 – Embedded security practical work

- **Team members:** BAALI Mohamed Rafik, MENASERI Habib
- **Team number:** 5
- **Final score:** 100 / 100 (Bus Master) – missions 1 to 8 validated

## How to run
Python 3.8+ is enough, nothing to install (standard library only; the figure in `docs/` was made with matplotlib).

```bash
python tp1_start.py
```

`TEAM = 5` is set at the top of `tp1_start.py`. The program completes the three decoding functions, runs the simulations (healthy bus, flooding attack), reads `logs/can_log_team05.csv` and prints the score.

## Result of the investigation
The intruder of team 5 uses identifier `0x200` (Braking) and injected 40 fake frames (190 observed, 150 expected in 3 s).
`tp1_start.py` also contains the timing detector of Q16 and an improved phase detector (bonus) that finds exactly the 40 fake frames.

## Structure
```
README.md
tp1_start.py     completed work file
tp1_common.py    given tools (not modified)
logs/            recording of team 5 only
docs/
  report.pdf     report
  fig_counts_intervals.png
```
