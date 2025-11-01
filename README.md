# IMDb Movie Data Analysis
Analyze the IMDb 5000 Movie Dataset using pandas, numpy, matplotlib, and seaborn. To view the analysis [click here](https://github.com/AdityaAgarwal1602/Movie-Data-Analysis/blob/main/imdb_movie_analysis.ipynb).

## Project highlights
- Clean budgets and gross revenue (strip $ and commas, coerce to numbers)
- Handle missing values and duplicates
- Feature engineer main_genre and profit
- Answer analyst-friendly questions with visuals:
	- Rating distribution (histogram)
	- Budget vs Gross (regression)
	- Ratings by Genre (boxplot)
	- Runtime trend since 1980 (line)
	- Top profitable directors (bar)
	- Correlation heatmap of key features

## Repository structure
- `Dataset/movie_metadata.csv` — Input dataset (kept local here; ensure it exists for the notebook/script).
- `imdb_movie_analysis.ipynb` — Jupyter notebook with markdown and plots.
- `imdb_movie_analysis.py` — Script version with `# %%` cells (run in VS Code or terminal).
- `requirements.txt` — Minimal dependencies to run the analysis.
- `.gitignore` — Ignores Python, Jupyter checkpoints, and common OS/IDE clutter.
- `LICENSE` — MIT License (edit your name/year if desired).

## Dataset
- Source: IMDb 5000 Movie Dataset (Kaggle)
- File used: `Dataset/movie_metadata.csv`
- Typical columns: `movie_title`, `director_name`, `genres`, `title_year`, `duration` (aka runtime), `budget`, `gross`, `imdb_score`, `num_voted_users`, etc.
- Note: Some numeric fields arrive as strings or contain zeros for missing values; the notebook/script handles cleaning and type coercion.

## Setup (Windows PowerShell)

1) Optional: Create and activate a virtual environment

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2) Install dependencies

```powershell
pip install -r requirements.txt
```

3a) Run the script

```powershell
python .\imdb_movie_analysis.py
```

3b) Or open the notebook

```powershell
jupyter notebook .\imdb_movie_analysis.ipynb
```

Notes:
- The code expects the CSV at `Dataset/movie_metadata.csv`. Adjust `csv_path` if yours differs.

## License
MIT — see `LICENSE`.
