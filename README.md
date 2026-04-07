# Emergent Models Experiments

This repository contains the code required to reproduce the experiments from the *Emergent Models* paper.

## Overview

The workflow is notebook-based. Running a specific task requires editing selected parts of the notebooks, with the relevant sections explained inline. The implementation is designed for large-scale simulations, and GPU acceleration through **Taichi** enables the batching of tens of thousands of emergent models (EMs).

## Dependencies

The required Python dependencies are:

- `numpy`
- `matplotlib`
- `taichi` with GPU support

## Typical Setup

The recommended environment is **Google Colab with GPU enabled**.

## Repository Structure

### `trainer.ipynb`
This notebook performs the actual training procedure and saves the resulting genome to a connected Drive folder.

Colab link: [Open `trainer.ipynb` in Google Colab](https://colab.research.google.com/drive/1wHB9oznsVTvKhhLG3_Wfe5gFsbbPQ-Cv?usp=sharing)

### `evaluator.ipynb`
This notebook handles evaluation and plotting. It requires access to the same Drive folder used by `trainer.ipynb`, since it reads the outputs produced during training.

Colab link: [Open `evaluator.ipynb` in Google Colab](https://colab.research.google.com/drive/1wT94_ewwT52tPrhRTujA7-r21WTGYUhw?usp=sharing)

## Notes

- Reproducing the reported results requires several manual setup adjustments.
- At the current stage, the reproduction workflow is not yet fully streamlined and may be unintuitive in some places.
- The notebooks include inline guidance on the main sections that typically need to be modified for a given task.
- If you encounter any issue during setup or reproduction, please contact the author.
- More robust and user-friendly versions of the codebase are planned for future releases.

## Contact

For any help, please contact the author at **bocchesegiacomo01@gmail.com**.
