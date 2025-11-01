# IMDb Movie Data Analysis

Analyze the IMDb Movies dataset using pandas, numpy, matplotlib, and seaborn. This repo is structured and ready for GitHub so recruiters can quickly review your work.

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
- In VS Code, you can run the `.py` file cell-by-cell using the Python extension.

## Ready-to-push Git commands

Initialize a repo, make the first commit, and push to a new GitHub repository (replace YOUR-REPO-URL):

```powershell
git init
git add .
git commit -m "Initial commit: IMDb analysis (notebook + script)"
git branch -M main
git remote add origin YOUR-REPO-URL
git push -u origin main
```

Tip: If you prefer storing the dataset outside the repo, keep `Dataset/` in `.gitignore` and add a short note in the README for where to place the file.

## Optional: Notebook outputs & diffs
- Keeping plot outputs in the notebook makes the repo more readable on GitHub, but can increase file size.
- To keep notebooks lean, consider clearing outputs before committing or using tools like `nbstripout`.

## License
MIT — see `LICENSE`.
