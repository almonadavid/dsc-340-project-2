# DSC 340 – Project 2: Model Comparison

**David Almona · DSC 340: Applied Machine Learning · Spring 2026**

Compare five scikit-learn classifiers across two datasets using `Pipeline` and `GridSearchCV`.

---

## Project Overview

| | Phase 1 | Phase 2 |
|---|---|---|
| **Notebook** | `phase_one.ipynb` | `phase_two.ipynb` |
| **Dataset** | HTRU2 Pulsar (`pulsar.csv`) | Forest Cover Type (`covtype_30k.csv`) |
| **Task** | Binary classification | 7-class classification |
| **Metric** | F1 (pulsar class) | Macro F1 |

Both phases run five models — Logistic Regression, KNN, Random Forest, SVM (RBF), and SVM (Linear) — through a scaler + classifier pipeline with 5-fold stratified cross-validation.

---

## Data

The two data files are **not included** in this repository (see `.gitignore`). Obtain them separately and place them in the project root:

```
dsc-340-project-2/
├── covtype_30k.csv   # 30,000-row sample of UCI Forest Cover Type
└── pulsar.csv        # HTRU2 pulsar dataset (17,898 rows)
```

---

## Environment Setup

**Requirements:** Python ≥ 3.12.6

1. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
```

2. Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

---

## Running the Analysis

Launch Jupyter and open the notebooks in order:

```bash
jupyter notebook
```

- Open **`phase_one.ipynb`** — Pulsar classification
- Open **`phase_two.ipynb`** — Forest Cover Type classification

Run all cells top to bottom (`Kernel → Restart & Run All`).