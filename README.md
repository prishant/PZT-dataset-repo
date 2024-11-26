# PZT Dataset

This repository provides spatiotemporal acoustic scans of PZT material sensors captured using a novel experimental setup involving point contact excitation and Coulomb coupling techniques. The dataset includes:

- [X_healthy.mat](.\X_healthy.mat): Acoustic scan of a PZT sensor under ideal conditions (healthy state).
- [X_damage.mat](.\X_damage.mat): Acoustic scan of the same sensor with introduced surface damage.

## Usage

The files are in `.mat` format for use in python:
```python
import scipy.io

mat1 = scipy.io.loadmat('X_healthy.mat')
healthy = mat1['healthyData'] # Load healthy sample data

mat2 = scipy.io.loadmat('X_damage.mat')
damage = mat2['damageData']  # Load damaged sample data
