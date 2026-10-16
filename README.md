# TTC subway delays

Academic data-mining project on the [TTC Subway Delay Data](https://open.toronto.ca/). The notebook follows the KDD process: selection, cleaning, transformation, mining and interpretation.

It covers the main causes, weekday and hour patterns, the lines and stations with the most delay, and passenger impact (`Min Delay` and `Min Gap`).

## Run

```bash
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
.venv/bin/jupyter lab src/ttc_subway_delay_kdd.ipynb
```

The notebook looks for `TTC Subway Delay Data since 2025.csv` in `src/`.

## Columns

| Column | Contents |
|---|---|
| `Date`, `Time`, `Day` | When the incident was logged |
| `Station`, `Line`, `Bound`, `Vehicle` | Where, and on which train |
| `Code` | TTC cause code |
| `Min Delay`, `Min Gap` | Minutes of delay, and the gap to the next train |
