Image Segmentation with Custom Loss and Representation Constraints

Overview

This project explores 3D volumetric image segmentation using PyTorch, with a focus on improving representation learning through custom loss functions and structural constraints in encoder-decoder architectures.
Key Ideas
* Convolution operates on local neighborhoods, transforming voxel-level vectors into higher-level representations
* Channel space represents feature vectors per voxel, not just scalar intensity
* Model enforces consistency between encoder and decoder representations
* Focus on sparsity-aware learning due to highly sparse input data (~85%)

Contributions
* Implemented a custom **Weighted Dice Loss** for imbalanced volumetric data
* Designed experimental normalization/activation strategy to stabilize feature magnitudes
* Explored representation consistency via encoder-decoder alignment
* Built 3D CNN pipeline for volumetric segmentation

Tech Stack
* Python
* PyTorch
* NumPy
* Medical imaging tools (nibabel)

Notes
This project is experimental and focuses on understanding representation learning dynamics rather than optimizing for benchmark performance.
