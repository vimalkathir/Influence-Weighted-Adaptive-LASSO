# Influence-Weighted Adaptive LASSO

## Research project

**Manuscript title:** *Influence-Weighted Adaptive LASSO: A Simulation Study of Variable Selection under Correlated Predictors and Data Contamination*

This repository accompanies a computational study comparing Ordinary LASSO, Elastic Net, Adaptive LASSO, and the proposed Influence-Weighted Adaptive LASSO (IWAL).

## Contents

- `LASSO.ipynb` — the Google Colab/Jupyter notebook containing the research code, exploratory real-data analysis, synthetic-data generation, model-fitting procedures, simulation framework, statistical comparisons, and figure-generation code.
- `Figure_Contamination_Comparison_Heatmap.png` — include this figure only if it is part of the final public research archive.

## Study design implemented in the notebook

The synthetic experiment is designed around:

- Sample size: 200 observations.
- Number of predictors: 20.
- Correlation levels: 0.0, 0.5, and 0.9.
- Contamination mechanisms: response, leverage, and cellwise contamination.
- Contamination levels: 5% and 10%, together with clean baseline conditions.
- Total conditions: 21.
- Replications per condition: 100.
- Methods compared: Ordinary LASSO, Elastic Net, Adaptive LASSO, and Influence-Weighted Adaptive LASSO.

The notebook also contains a preliminary real-data illustration using the diabetes dataset available through scikit-learn.

## Software requirements

The notebook imports the following Python packages:

- NumPy
- pandas
- SciPy
- scikit-learn
- Matplotlib
- seaborn
- Google Colab utilities (only for Colab-specific mounting or downloading operations)

A typical environment can install the principal scientific packages with:

```bash
pip install numpy pandas scipy scikit-learn matplotlib seaborn jupyter
```

The exact package versions used for the final archived analysis should be recorded before publication. This README does not claim fixed package versions because they are not recorded as a reproducible environment specification in the supplied notebook.

## Running the notebook

1. Open `LASSO.ipynb` in Google Colab or Jupyter Notebook.
2. Install the required packages if they are not already available.
3. Run the notebook cells in their intended order, checking the cell descriptions and dependencies.
4. The full simulation and analysis sections may take substantial time to execute.
5. Save the generated result files and figures to a persistent location before closing or disconnecting the runtime.

**Important:** The notebook uses temporary Colab paths such as `/content/LASSO_Final_Research_Results`. Files saved only under `/content/` may be lost when the runtime is reset. Copy the completed result folder to Google Drive or download it before ending the session.

## Reproducibility and result files

The notebook contains code to generate and analyse the simulation results, including performance summaries, selection frequencies, stability summaries, paired statistical tests, and the contamination-comparison heatmap.

The original results folder was not included with the notebook supplied for preparing this README. Therefore, the CSV result files are not currently archived alongside this README. They should be added to the repository or to a linked research-data archive if the journal or research plan requires the numerical outputs to be publicly available.

The notebook contains saved cell outputs, but saved notebook outputs should not be treated as a substitute for separately archived CSV files.

## Code availability

The public repository URL and the permanent archive DOI will be added here after the repository is created and a version is archived.

- GitHub repository: *to be added*
- Archived code DOI: *to be added*

## Citation

A formal software citation will be added after the Zenodo archive has generated a DOI.

## Notes

This repository is intended to support transparency and reproducibility of the computational procedures described in the accompanying manuscript. The interpretation of the results should follow the manuscript, including its stated limitations.
