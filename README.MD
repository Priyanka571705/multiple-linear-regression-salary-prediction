
# Hiring — Salary Prediction (Multiple Linear Regression)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-%20-blue?logo=pandas&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%20-orange?logo=scikit-learn&logoColor=white) ![matplotlib](https://img.shields.io/badge/matplotlib-%20-blue?logo=matplotlib&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-%20-orange?logo=jupyter&logoColor=white) ![VSCode](https://img.shields.io/badge/VS%20Code-%20-007ACC?logo=visual-studio-code&logoColor=white)

Professional summary
--------------------
This folder contains a hands-on implementation of a Multiple Linear Regression workflow to predict employee salaries using features such as years of experience, test score, and interview score. The project is delivered as an annotated Jupyter notebook suitable for developers who want to inspect the preprocessing, model training, evaluation and example prediction flow.

Repository contents
-------------------
- `hiring.csv` — dataset used for training and demonstration.
- `Multiple_Linear_Regression.ipynb` — annotated Jupyter notebook with code cells, plots and a simple interactive prediction example.

Key features
------------
- End-to-end EDA and preprocessing (missing-value handling, text-to-number conversion).
- Model training using `sklearn.linear_model.LinearRegression`.
- Inline plotting for Actual vs Predicted comparison and model diagnostics.
- Simple CLI-style input cells showing how to obtain on-demand predictions.

Tech stack
----------
- Language: Python 3.8+
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `word2number`, `jupyter`

Developer quickstart
--------------------
1. Clone and open the project folder:

```bash
git clone <your-repo-url>
cd Data-Science-project/Hiring
```

2. (Recommended) Create an isolated environment and install dependencies (Windows example):

```bash
python -m venv venv
venv\Scripts\activate
pip install --upgrade pip
pip install pandas numpy scikit-learn matplotlib seaborn jupyter word2number
```

3. Launch the notebook and run cells sequentially:

```bash
jupyter notebook Multiple_Linear_Regression.ipynb
```

Reproducibility & extension notes
--------------------------------
- The notebook performs preprocessing inline. For production or repeated use, extract transformation steps into `src/preprocessing.py` and add unit tests.
- Pin dependencies with `pip freeze > requirements.txt` or provide an `environment.yml` for conda.
- Replace interactive `input()` cells with function-based inference for automated testing or CI.

Suggested next steps for maintainers
----------------------------------
- Add a `requirements.txt` with pinned versions and a short `Makefile` or `run.sh` wrapper.
- Export key plots to `reports/` and include a one-page executive summary.
- Add a lightweight test that validates preprocessing (e.g., converting experience text to numeric values) and model prediction shape.

Files of interest
-----------------
- Notebook: [Multiple_Linear_Regression.ipynb](Data-Science-project/Hiring/Multiple_Linear_Regression.ipynb)
- Dataset: [hiring.csv](Data-Science-project/Hiring/hiring.csv)

License
-------
See repository root for license information. This content is provided for demonstration and learning purposes.

Need help?
----------
I can: generate a `requirements.txt`, extract preprocessing into a reusable module, or run the notebook and export example charts — tell me which you'd prefer.

