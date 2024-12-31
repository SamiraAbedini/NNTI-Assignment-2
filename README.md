# Neural Network and Transfer Learning: Assignment 2

This repository contains solutions to **Assignment 2** of the Neural Network and Transfer Learning course. The assignment is divided into two main exercises: implementing custom `Dataset` and `DataLoader` classes in PyTorch, and performing Principal Component Analysis (PCA) for image reconstruction using Eigen Decomposition (EVD) and Singular Value Decomposition (SVD).

## Table of Contents
- [Overview](#overview)
- [Exercise 2.2 - Datasets and Dataloaders](#exercise-22---datasets-and-dataloaders)
- [Exercise 2.3 - Eigencats](#exercise-23---eigencats)
- [Getting Started](#getting-started)
- [Results](#results)
- [Contributors](#contributors)
- [License](#license)

---

## Overview

### Exercise 2.2: Datasets and Dataloaders
This exercise focuses on creating custom PyTorch `Dataset` and `DataLoader` classes for two datasets. The implementation demonstrates:

1. **Dataset1 - Tokenized SMS Messages:**
   - Tokenized text data (SMS messages labeled as spam or not spam).
   - Processed to include padding for uniform input size.
   - Binary labels (0 for not spam, 1 for spam).
   - Implemented a custom `Dataset` class to preprocess the data and a `DataLoader` to batch and shuffle it.

2. **Dataset2 - Vector-borne Disease Data:**
   - Tabular data containing symptoms and prognoses.
   - Labels encoded using one-hot encoding.
   - Created a custom `Dataset` class to preprocess the tabular data, handle categorical encoding, and manage data splits.

### Exercise 2.3: Eigencats
This exercise demonstrates Principal Component Analysis (PCA) applied to a dataset of cat images. Key aspects include:

1. **Computing the Mean Cat:**
   - Calculated the mean image by averaging pixel values across all samples.
   - Visualized the result to understand the average characteristics of the dataset.

2. **Eigencats - Principal Components of Images:**
   - Used Eigen Decomposition (EVD) to compute the principal components (eigencats).
   - Visualized the top principal components as "eigenfaces" for cats.

3. **Reconstructing Images:**
   - Reconstructed images using varying numbers of principal components.
   - Demonstrated image fidelity improvement with additional components.
   - Used Singular Value Decomposition (SVD) as an alternative method for PCA and compared its results to EVD.

---

## Getting Started

### Prerequisites
- Python 3.6 or higher
- PyTorch
- Numpy
- Matplotlib
- Pandas

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/username/NNTI_Assignment2.git
   ```
2. Navigate to the repository:
   ```bash
   cd NNTI_Assignment2
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Code
- **Dataset and Dataloader Implementation:** Execute `exercise_2_2.py` to see the custom `Dataset` and `DataLoader` classes in action.
- **Eigencats Analysis:** Open `exercise_2_3.ipynb` and run the notebook to see PCA-based image reconstruction.

---

## Results

### Datasets and Dataloaders
- **Dataset1:** Successfully tokenized, padded, and batched SMS messages with their corresponding labels.
- **Dataset2:** Successfully preprocessed tabular data, applied one-hot encoding, and loaded data for analysis.

### Eigencats
- **Mean Cat:** Visualized the average image of the dataset.
- **Principal Components:** Computed and visualized top eigencats using both EVD and SVD.
- **Reconstructed Images:**
  - Visualized reconstructed images with varying numbers of principal components (e.g., 10, 40, and 80 components).
  - Observed trade-offs between reconstruction quality and the number of components used.

#### Example Output
1. **Mean Cat Image:**
   ![Mean Cat](imgs/meancat.png)
2. **Reconstructed Images (10, 40, 80 Singular Values):**
   ![Reconstructed Cats](imgs/reconstructed_cats.png)

---


