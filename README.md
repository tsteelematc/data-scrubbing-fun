# data-scrubbing-fun

This project computes a language ranking from `data.csv` using a naive metric:

`naive_speakers_per_country = Number of speakers / country_count`

Where `country_count` is derived by splitting `Countries` on commas and trimming whitespace. Rows with empty `Countries` are excluded.

## Setup (uv project + venv)

```bash
uv sync
```

## Run the notebook

```bash
uv run jupyter notebook
```

Then open `language_ranking.ipynb` and run all cells.

The notebook writes a reproducible full ranking CSV to:

`outputs/language_rankings_by_naive_speakers_per_country.csv`
