# Airline EDA – GitHub Setup

This repo tracks your assignment notebook while keeping noise (checkpoints, outputs) out of Git.

## Suggested structure
```
airline-eda/
├─ notebooks/
│  └─ exploratory_data_analysis.ipynb
├─ data/                # put airline_dataset.csv here (ignored by default)
├─ reports/             # export PDF here (ignored)
├─ README.md
└─ .gitignore
```

## Quick start
```bash
# 1) initialize repo
git init
git add .
git commit -m "Initial commit: EDA notebook template"

# 2) set your identity
git config user.name "Your Name"
git config user.email "you@example.com"

# 3) create GitHub repo (on github.com) and add it as remote
git remote add origin https://github.com/<YOUR_USER>/<YOUR_REPO>.git
# or (recommended) use SSH after adding your SSH key to GitHub:
# git remote add origin git@github.com:<YOUR_USER>/<YOUR_REPO>.git

# 4) push
git branch -M main
git push -u origin main
```

## Tips
- **Keep data local**: `data/*.csv` is ignored by default. Remove that line in `.gitignore` if you need to track the CSV (only if it's small and permitted).
- **Cleaner diffs**: install [nbdime] to see meaningful notebook diffs:
  ```bash
  pip install nbdime
  nbdime config-git --enable
  ```
- **Strip outputs before commit (optional)** to reduce repo size:
  ```bash
  pip install nbstripout
  nbstripout --install
  ```
- **PDF export**: export your notebook to PDF into `reports/` and keep the `.ipynb` in `notebooks/`.
