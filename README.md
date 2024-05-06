## Species identification of microbial eukaryotes with Raman spectroscopy

In the jupyter notebook you can find the code for this project and some exemplary visualisaiton.
The input data is expected to follow this structure:

```
species_dir
│
├── bg
│    ├── spectra_0.txt
│    │       ...
│    └── spectra_N.txt 
├── cell_0
│    ├── spectra_0.txt
│    │       ...
│    └── spectra_N.txt 
├── cell_1
...
```

### The processing steps include:
- background subtraction 
- cosmic ray filtering
- smoothing
- interpolation
- normalisaiton

### The analysis steps include:
- PCA
- SVM \
The data for model is split using scikit-learn splitter (train 70%, test 30%).

### In the end results are visualised using:
- UMAP plot
- confusion matrix of prediciton results

