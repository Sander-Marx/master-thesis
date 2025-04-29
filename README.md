# Master thesis
This repository contains code for Sander Marx's master thesis, "Learning acoustic target classification from simulation". \
The thesis explored deep learning techniques to classify underwater acoustic targets using simulated training data and real-world measurements. Experiments were conducted to explore how effectively models trained primarily on simulated data can generalize to real-world scenarios.



### Data
The data is availaibe in a compressed folder from this link: \
https://drive.google.com/uc?export=download&id=1JGIbmhM-3w1inivs6t9Jbr_AD2J1b0cb

1. Download the compressed folder from the link above
2. Extract the contents
3. Place the two extracted CSV files in the `Data` folder

### Experiments

The `Experiments` folder contains Jupyter notebooks for the two main experiments:

**Experiment 1: Simulated Data Classification**
- `experiment1_1D_hybrid_conv.ipynb`: Implementation of the hybrid convolutional model.
- `shallow_models_comparison_experiment1.ipynb`: Comparative analysis of traditional ML models.

**Experiment 2: Transfer to Real-World Data**
- `experiment2_1D_conv_in_situ.ipynb`: Application of 1D convolutional networks to in-situ measurements.


## Plot
The `Plot` folder contains two notebooks:

- `data_explore.ipynb`: Analysis and visualization of the simulated data distributions.
- `plot_pred_vs_measured_experiment2.ipynb`: Comparative plots of the 12 real-world measured target strength spectra against the model predictions.



## Other folders
- `Models` folder: Trained PyTorch model files (`.pth`) for both experiments.
- `in_situ_data` folder: Real-world acoustic measurements from 12 targets used as test data for Experiment 2
- `grid_search` folder: CSV files containing hyperparameter combinations and corresponding validation performance metrics


## Requirements

The codebase requires Python 3.9+ with the following packages:

- PyTorch
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

`requirements.txt` contains the versions of these packages.
