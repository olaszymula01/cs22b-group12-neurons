# How Do Neurons Differ? Electrical Properties of Human and Mouse Brain Cells

CS 22B, Fall 2026 · Team 12: Aleksandra (Ola) Szymula, Fatima Garcia, Carolyna Sias

**Main question:** How do the electrical properties of neurons differ between species (human vs. mouse) and cell types (spiny vs. aspiny)?

## Data

- **Source:** Allen Institute for Brain Science, Allen Cell Types Database: https://celltypes.brain-map.org
- **File:** https://celltypes.brain-map.org/cell_types_specimen_details.csv
- **One row = one neuron** recorded in a slice of mouse or human brain tissue.

Opening the file link downloads the CSV. Save it as `data/cell_types_specimen_details.csv`.

## Notebooks

| Notebook | What it does | Lead |
| --- | --- | --- |
| `01_loading_and_cleaning.ipynb` | Loads and inspects the raw file, cleans it, saves `data/neurons_clean.csv` | Ola |
| `02_analysis.ipynb` | Filtering, grouping and aggregation on the cleaned data | Fatima |
| `03_visualizations.ipynb` | Plots and interpretation | Caro |

Run `01_loading_and_cleaning.ipynb` first. The other notebooks read `data/neurons_clean.csv`, which it creates. For the final submission, the three parts are combined into one notebook.

## Running in Google Colab

1. Open the notebook in Colab (File → Open notebook → GitHub tab, then paste the repo URL).
2. In the Files panel on the left, create a folder named `data`.
3. Upload `cell_types_specimen_details.csv` into that folder.
4. Run all cells (Runtime → Run all).

Colab deletes uploaded files when the session ends, so repeat steps 2 and 3 each time.

## Running in Jupyter

Clone the repo, put the CSV in `data/`, and run the notebook from the repo folder.

## Libraries

pandas, NumPy, matplotlib, seaborn. All are already installed in Google Colab.
