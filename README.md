# How Do Neurons Differ? Electrical Properties of Human and Mouse Brain Cells

CS 22B, Fall 2026 · Team 12: Aleksandra (Ola) Szymula, Fatima Garcia, Carolyna Sias

**Main question:** How do the electrical properties of neurons differ between species (human vs. mouse) and cell types (spiny vs. aspiny)?

## Data

- **Source:** Allen Institute for Brain Science, Allen Cell Types Database: https://celltypes.brain-map.org
- **File:** https://celltypes.brain-map.org/cell_types_specimen_details.csv
- **One row = one neuron** recorded in a slice of mouse or human brain tissue.

`01_loading_and_cleaning.ipynb` downloads this file into `data/` automatically the first time it runs, so you don't need to download it yourself.

## Notebooks

| Notebook | What it does | Lead |
| --- | --- | --- |
| `01_loading_and_cleaning.ipynb` | Loads and inspects the raw file, cleans it, saves `data/neurons_clean.csv` | Ola |
| `02_analysis.ipynb` | Filtering, grouping and aggregation on the cleaned data | Fatima |
| `03_visualizations.ipynb` | Plots and interpretation | Caro |

Run `01_loading_and_cleaning.ipynb` first. The other notebooks read `data/neurons_clean.csv`, which it creates. For the final submission, the three parts are combined into one notebook.

## Running in Google Colab

1. Open the notebook in Colab (File → Open notebook → GitHub tab, then paste the repo URL).
2. Run all cells (Runtime → Run all). The first cell downloads the data.

The other notebooks need `data/neurons_clean.csv`. Colab deletes files when the session ends, so in a new session run `01_loading_and_cleaning.ipynb` first, in the same session.

## Running in Jupyter

Clone the repo and run the notebook from the repo folder. The data downloads on the first run.

## Libraries

pandas, NumPy, matplotlib, seaborn. All are already installed in Google Colab.
