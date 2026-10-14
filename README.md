# DSCI 552 Homework 2

Hongwei Xiao | GitHub: Ga9a

The notebook covers regression and KNN on the Combined Cycle Power Plant dataset,
plus ISLR Section 2.4, Exercises 1 and 7. It includes executed outputs and written answers.

## Files

- `notebooks/Xiao_Hongwei_HW2.ipynb`: completed homework.
- `data/CCPP/Folds5x2_pp.xlsx`: original dataset; the notebook uses Sheet 1 only.
- `data/CCPP/Readme.txt`: original dataset description and references.
- `requirements.txt`: versions of the direct dependencies used for verification.

## Run

Use Python 3.12. From the repository root, install the dependencies and start JupyterLab:

```sh
python -m pip install -r requirements.txt
python -m jupyterlab notebooks/Xiao_Hongwei_HW2.ipynb
```

Select the matching Python kernel, restart it, and run all cells in order.
The notebook reads the data with a relative path from the `notebooks` directory.
Parts (h)-(j) share a 70/30 split with `random_state=42`.
KNN normalization uses training-set minima and maxima.

AI assistance is documented at the end of the notebook.

## Reproducibility checks

Use Python 3.12 with the pinned dependencies. The submitted notebook preserves its recorded analysis; the verification script checks notebook structure and saved errors without changing it.

```sh
python scripts/verify_notebook.py
python scripts/verify_notebook.py --execute
```

Execution uses the notebook directory as its working directory, so dataset paths resolve consistently. Run the command in the environment where the requirements were installed. CI reruns all code cells on a clean checkout. Generated results written by notebook code may be refreshed during execution.
