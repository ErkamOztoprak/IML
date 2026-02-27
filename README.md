# IML — Introduction to Machine Learning 📘

Collection of Jupyter notebooks covering introductory machine learning concepts, experiments, and exercises.

## Overview

This repository contains a sequence of notebooks (w1..w7) that introduce core machine learning topics with hands-on examples. Notebooks include data loading, preprocessing, supervised learning (regression/classification), model evaluation, and visualization.

## Contents

- `w1/` — Week 1: Data exploration & preprocessing
- `w2/` — Week 2: Linear models & regression
- `w3/` — Week 3: Classification basics
- `w4/` — Week 4: Model evaluation & validation
- `w5/` — Week 5: Feature engineering
- `w6/` — Week 6: Ensemble methods
- `w7/` — Week 7: Final project / advanced topics

(Adjust the folder descriptions if your notebooks follow a different structure.)

## Quick Start

Recommended Python version: 3.9+ (3.10+ preferred)

Create a virtual environment and install dependencies:

```bash
python -m venv .venv
# Windows
.\.venv\Scripts\Activate.ps1   # PowerShell
# or
.\.venv\Scripts\activate.bat   # cmd
# macOS / Linux
source .venv/bin/activate

pip install --upgrade pip
pip install jupyter pandas numpy scikit-learn matplotlib seaborn notebook
```

If the repository includes a `requirements.txt`, install with:

```bash
pip install -r requirements.txt
```

Start Jupyter Notebook/Lab:

```bash
jupyter notebook
# or
jupyter lab
```

Open the notebooks in your browser and run the cells interactively.

## Suggested Dependencies

- Python 3.9+
- numpy
- pandas
- scikit-learn
- matplotlib
- seaborn
- jupyter or jupyterlab
- notebook

Optionally:
- plotly (interactive plots)
- tensorflow / pytorch (if any deep learning notebooks exist)

## Running & Exporting

To run a notebook headlessly and export to HTML (useful for CI or sharing):

```bash
# Execute notebook and save output to HTML using nbconvert
jupyter nbconvert --to html --execute w1/your_notebook.ipynb
```

To run a whole folder of notebooks (simple loop):

```bash
for nb in w*/**/*.ipynb; do
  jupyter nbconvert --to html --execute "$nb" || break
done
```

(Windows PowerShell users can adapt the loop accordingly.)

## Notes for Contributors

- Keep notebooks reproducible: set random seeds where appropriate and clearly specify dataset paths.
- Add a brief markdown summary at the top of each notebook explaining goals and inputs/outputs.
- Keep long-running experiments in separate notebooks or provide saved outputs to avoid rerun cost.

## License

If not specified in the repository, add a `LICENSE` file (MIT recommended for educational materials).

## Contact

For questions, open an issue in the repository.

---

*This README was generated to provide a clear introduction and usage instructions for the IML notebook collection.*
