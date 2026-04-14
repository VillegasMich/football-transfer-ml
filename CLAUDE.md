# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

University ML project: **Predicción del Valor de Mercado de Jugadores de Fútbol** (Football Player Market Value Prediction). The goal is to predict `market_value_in_eur` from football transfer records.

## Dataset

`transfers.csv` — 157,186 rows of football transfer records with these columns:
- `player_id`, `player_name`
- `transfer_date`, `transfer_season`
- `from_club_id`, `from_club_name`, `to_club_id`, `to_club_name`
- `transfer_fee` — 54,833 missing values
- `market_value_in_eur` — 60,848 missing values (the prediction target)

## Development

All work lives in `main.ipynb` (Jupyter notebook). To run it:

```bash
jupyter notebook main.ipynb
# or
jupyter lab
```

Install dependencies (none declared yet — add as needed):
```bash
pip install pandas scikit-learn jupyter matplotlib seaborn
```

## Language

Interactions with Claude may be in Spanish, but all generated content must be in English — this includes code, variable names, markdown text, and comments.

## Notes

- The PDF (`Entrega Preliminar...pdf`) contains the preliminary project report and requirements.
- The notebook is currently empty — development is in early stages.
- Target variable has ~39% missing values; preprocessing strategy for these rows is a key design decision.
