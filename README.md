# Big Data Cup 2025 — Hockey Tracking Analytics

Code, data products, and research materials from the 2025 Big Data Cup analytics competition, hosted by Stathletes, the Rotman School of Management, and the University of Toronto Sports Analytics Student Group (UTSPAN).

## Project structure

- `notebooks/` — numbered analyses, ordered from event preparation through coverage and visualization work
- `data/derived/` — cleaned tracking, shift, coverage, and penalty-play CSV outputs
- `assets/figures/` — exported visuals for reports and presentations
- `src/` — reusable analysis modules as the project is further productionized
- `paper/` — final competition manuscript
- `environment/` — Python and R dependency references

## Notebook guide

1. `01_filter_events.ipynb` — event, shift, and tracking-data filtering
2. `02_synchronization.ipynb` — event/tracking synchronization
3. `03_coverage_analysis.ipynb` — puck and player coverage analysis
4. `04_coverage_validation.ipynb` — coverage-analysis variant and validation
5. `05_play_gif_generation.Rmd` — animated play visualizations

## Setup

Python notebooks require the packages in `requirements.txt`. The R notebook uses the packages listed in `environment/r-packages.txt`.

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\\Scripts\\activate
pip install -r requirements.txt
```

## Data

Derived competition outputs are included under `data/derived/`. Some notebooks reference original Big Data Cup source exports or Google Drive paths that are not committed here. Supply authorized raw exports under `data/raw/` and update those notebook paths before re-running the full workflow.

## Research paper

The final manuscript is available at `paper/big_data_cup_2025_paper.pdf`.
