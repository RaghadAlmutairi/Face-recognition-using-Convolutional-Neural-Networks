ANN Project — Olivetti Faces (CNN Experiments)
===============================================

**Project**: Classification experiments using Convolutional Neural Networks (CNNs) on the Olivetti/ORL face dataset. The main working file is the notebook `ANN_project (1).ipynb`.

**Purpose**:
- Explore the dataset and visualize samples.
- Build and train several CNN architectures.
- Answer guided questions (Q1–Q10) about architecture choices, pooling sizes, batch size effects, and training curves.

**Requirements**:
- Python 3.8+ (recommended)
- Packages: `numpy`, `matplotlib`, `scikit-learn`, `tensorflow` (or `keras`), `jupyter`

Quick setup (PowerShell):
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install numpy matplotlib scikit-learn tensorflow jupyter
```

Optional `requirements.txt` (example):
```
numpy
matplotlib
scikit-learn
tensorflow
jupyter
```

**How to run**:
- Activate your virtual environment (see above).
- Start Jupyter Notebook from this folder:
```powershell
jupyter notebook
```
- Open `ANN_project (1).ipynb` and run the cells in order. If you run the notebook locally, update the dataset load paths in the early cells (replace `/content/` with `./` or the actual path to the `.npy` files).

**Notebook structure (high level)**:
- Data loading and shape checks
- Visualization: sample images and per-subject samples
- Train/validation/test splitting and reshape for Keras
- Several CNN architectures (including experiments with pooling size, number of filters, dense units)
- Training runs (batch size 32 and 16, different epoch counts)
- Plots for training vs validation accuracy and difference per epoch
- Final evaluation on validation/test splits
