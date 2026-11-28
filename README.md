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
| `team12_final_notebook.ipynb` | **Combined notebook (draft):** Part 1 cleaning, Part 2 analysis, Part 3 plots, conclusion | All |
| `01_loading_and_cleaning.ipynb` | Part 1 on its own: loads and inspects the raw file, cleans it, saves `data/neurons_clean.csv` | Ola |
| `02_grouping_and_analysis.ipynb` | Parts 1 and 2: filtering, grouping and aggregation on the cleaned data | Fatima |

`team12_final_notebook.ipynb` is the one to submit. It runs from start to finish on its own. Part 3 (plots, led by Caro) and the conclusion are still to be filled in.

## Running in Google Colab

1. Open the notebook in Colab (File → Open notebook → GitHub tab, then paste the repo URL).
2. Run all cells (Runtime → Run all). The first cell downloads the data.

The other notebooks need `data/neurons_clean.csv`. Colab deletes files when the session ends, so in a new session run the cleaning part first, in the same session.

## Running in Jupyter

Clone the repo and run the notebook from the repo folder. The data downloads on the first run.

## Libraries

pandas, NumPy, matplotlib, seaborn. All are already installed in Google Colab.
