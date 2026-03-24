Representation Learning in 3D CNNs (Experimental)

Overview

This repository contains a set of experiments exploring representation learning in neural networks, with a focus on 3D convolutional architectures, sparsity, and feature consistency.

The work is driven by a core question: How do neural networks represent structured data across layers, and how can we constrain or guide this representation?
Rather than focusing only on performance, these experiments investigate the internal behavior of models—especially how feature vectors evolve through convolution, normalization, and training.

---

Key Areas Explored

1. 3D Convolutional Representation

* Input data is treated as a volumetric space where each voxel contains a feature vector (channel space)
* Convolution is interpreted as a transformation from local neighborhoods into higher-level representations
* Emphasis on how spatial and channel dimensions interact

2. Sparse Data Learning

* Experiments assume highly sparse inputs (~80–90% near-zero regions)
* Models are analyzed for how sparsity propagates through layers
* Focus on maintaining meaningful signal while suppressing noise

3. Custom Loss Functions

* Implementation of **Weighted Dice Loss** for imbalanced segmentation tasks
* Designed to handle sparse targets and improve stability in training

4. Normalization and Activation

* Exploration of custom normalization strategies
* Aim: stabilize feature magnitudes while preserving learned structure
* Investigates how activation impacts representation consistency

5. Encoder–Decoder Consistency

* Study of how features learned in encoder layers relate to decoder reconstruction
* Experimental ideas around preserving structural coherence across layers

---

Repository Structure

* `nnclassificationexp.ipynb`
  Experiments with neural network classification and feature learning

* `compv_imgseg.ipynb`
  3D image segmentation pipeline using convolutional neural networks

* `weighteddice.ipynb`
  Implementation and testing of weighted Dice loss for segmentation

* `normalizedActivation.ipynb`
  Experiments with custom normalization and activation behavior


Tech Stack

* Python
* PyTorch
* NumPy
* (Optional) Medical imaging tools like nibabel

---

Approach

This repository is exploratory rather than production-oriented.

Instead of using models as black boxes, the focus is on:

* understanding how representations are formed
* analyzing how information propagates
* experimenting with constraints on learning dynamics

---

Notes

* These experiments are not optimized for benchmark performance
* Some ideas are speculative and under active exploration
* The goal is to build intuition around deep learning systems from first principles

---

Author

Self-taught developer with a focus on:

* Machine Learning
* Mathematical foundations of learning systems
* Representation learning and model behavior
