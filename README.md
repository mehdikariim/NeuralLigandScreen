# NeuralLigandScreen

A Jupyter notebook for ligand-based screening using neural networks to predict pIC50 values for EGFR inhibitors based on ChEMBL data. The project includes data preprocessing, neural network training, evaluation, and prediction on external data, with visualizations of predicted pIC50 values and molecular structures.

## Features
- Converts SMILES strings to MACCS fingerprints for molecular encoding.
- Trains a neural network with two hidden layers to predict pIC50 values.
- Evaluates model performance with MSE and MAE metrics.
- Predicts pIC50 values for external compounds and visualizes the top three candidates.

## Requirements
- Python 3.9+
- Libraries: `pandas`, `numpy`, `rdkit`, `keras`, `scikit-learn`, `matplotlib`, `seaborn`
- Input files:
  - `EGFR_compounds_new.csv`: ChEMBL data with `smiles` and `pIC50` columns (not included in this repository).
  - `test.csv`: External test data with `canonical_smiles` column (not included in this repository).

## Installation
Run the first cell in `NeuralLigandScreen.ipynb` to install dependencies using `condacolab` and `mamba` in a Colab environment. For local setup, install the required libraries:
```bash
conda install -c conda-forge pandas matplotlib seaborn rdkit
pip install --upgrade keras scikit-learn
