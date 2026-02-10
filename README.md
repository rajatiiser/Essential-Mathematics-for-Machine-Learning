## Image Compression using Singular Value Decomposition (SVD)

### Overview
This project demonstrates image compression using Singular Value Decomposition
based on low-rank matrix approximation. By retaining only the top-k singular
values, the image can be reconstructed with reduced storage while preserving
visual quality.

### Mathematical Background
An image is represented as a matrix A ∈ ℝ^(m×n).
Using SVD:
A = U Σ Vᵀ

Low-rank approximation:
A_k = U_k Σ_k V_kᵀ

where k ≪ min(m, n).

### Methodology
- Convert image to grayscale
- Compute SVD
- Reconstruct image using top-k singular values
- Compare visual quality and compression effect

### Results
- Visual comparison for k = 5, 50, 100, 650
- Singular value decay plot
- Discussion of compression vs reconstruction quality

### Tools Used
- Python
- NumPy
- Matplotlib
- Jupyter Notebook

### Conclusion
SVD-based compression demonstrates that most visual information in images
is captured by a small number of singular values. This validates the use
of low-rank approximation for efficient image storage.
