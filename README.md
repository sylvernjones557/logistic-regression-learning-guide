# Machine Learning Learning Guide

This repository turns the original Jupyter notebooks into a structured study
path for supervised and unsupervised machine learning.

## Learning path

| Order | Notebook | Main idea |
| --- | --- | --- |
| 1 | `01-logistic-regression.ipynb` | Binary classification with logistic regression |
| 2 | `02-k-nearest-neighbors.ipynb` | Distance-based classification |
| 3 | `03-support-vector-machine.ipynb` | Maximum-margin classification |
| 4 | `04-decision-tree.ipynb` | Rule-based classification |
| 5 | `05-random-forest.ipynb` | Ensemble learning with decision trees |
| 6 | `06-hyperparameter-tuning-basic.ipynb` | Searching for better model settings |
| 7 | `07-hyperparameter-tuning-comparison.ipynb` | Comparing tuning approaches |
| 8 | `08-k-means-clustering.ipynb` | Centroid-based unsupervised learning |
| 9 | `09-dbscan-clustering.ipynb` | Density-based unsupervised learning |
| 10 | `10-logistic-regression-exploration.ipynb` | Additional logistic-regression practice |

The notebooks use the sample heart-disease dataset in
`data/heart_disease.csv`. The `archive/originals` directory preserves the
original files, including notebooks that were not part of the main learning
sequence.

## Setup

From this repository's root directory:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
jupyter notebook
```

Open the `notebooks` directory and follow the numbered order. If PowerShell
blocks activation, run the notebooks with the Python environment that has the
packages from `requirements.txt` installed.

## Git workflow

```powershell
git clone https://github.com/<owner>/<repository>.git
cd logistic-regression-learning-guide
git pull
```

After making changes:

```powershell
git add .
git commit -m "Update machine learning notes"
git push
```

Do not commit passwords, API keys, tokens, virtual environments, or large
generated files.
