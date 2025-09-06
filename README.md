# KNN Imputation: NumPy vs PyTorch

This repo contains a single notebook comparing KNN-based missing value imputation using:

- **NumPy (CPU)**

- **PyTorch (CPU)**

- **PyTorch (CUDA)**

## What the code does

- Finds the best feature set (X) for each target column (Y).

- Tests different feature set sizes (best **3, 4, and 5 Xs** for each Y).

- Compares runtime performance between NumPy (CPU), PyTorch (CPU), and PyTorch (CUDA).

| Method         | Features | Runtime (s) |
| -------------- | -------- | ----------- |
| NumPy (CPU)    | 3 of 10  | **220.7**   |
| NumPy (CPU)    | 4 of 10  | **400.8**   |
| NumPy (CPU)    | 5 of 10  | **517.6**   |
| PyTorch (CPU)  | 3 of 10  | **233.1**   |
| PyTorch (CPU)  | 4 of 10  | **366.3**   |
| PyTorch (CPU)  | 5 of 10  | **460.9**   |
| PyTorch (CUDA) | 3 of 10  | **6.8**     |
| PyTorch (CUDA) | 4 of 10  | **11.9**    |
| PyTorch (CUDA) | 5 of 10  | **14.09**   |
⚡ GPU acceleration (CUDA) provides a dramatic speedup compared to CPU.

## Notes

- Full explanation and methodology are in my article.

- This repo only provides the supporting code and benchmark results.

