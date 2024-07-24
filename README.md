# Face Recognition using Principal Component Analysis (PCA)

This project implements a basic facial recognition system using Principal Component Analysis (PCA) by projecting face images onto a feature space known as the "Eigenfaces". The system recognizes a person's face by comparing it to a pre-existing database of faces and identifying the closest match.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Tasks](#tasks)
- [Implementation](#implementation)
- [Results](#results)
- [Usage](#usage)
- [References](#references)

## Introduction

Principal Component Analysis (PCA) is a statistical technique that transforms possibly correlated variables into a set of linearly uncorrelated variables called principal components. In the context of facial recognition, PCA is used to reduce the dimensionality of the face images while preserving the variation in the dataset.

The face space is defined by the "Eigenfaces", which are the eigenvectors of the set of face images. The goal of this project is to recognize a person's face by comparing it to a pre-existing database of faces and identifying the closest match.

## Dataset

The AT&T face dataset contains a set of grayscale face images with dimensions 92x112 pixels. The images are organized in 40 directories (one for each subject), named `sX` where `X` indicates the subject number (1 to 40). Each directory contains ten different images of the subject, named `Y.pgm` where `Y` is the image number (1 to 10). These images vary in lighting, facial expressions, and facial details.

- [Link to AT&T face dataset](https://git-disl.github.io/GTDLBench/datasets/att_face_dataset/)

## Tasks

1. **Load Dataset**: Load the dataset and divide it into training and test sets.
2. **Implement PCA**: Implement the PCA algorithm from scratch.
3. **Image Reconstruction**: Implement image reconstruction using eigen projections and visualize differences for different numbers of components.
4. **Visualize Mean Face**: Visualize the mean (Eigenface) generated.
5. **Face Recognition**: Given the training set, obtain accuracy by attempting a face recognition module and obtaining accuracy for different numbers of principal components.

## Implementation

### 1. Load Dataset

Load the AT&T face dataset and split it into training and test sets. 

### 2. Implement PCA

Implement PCA to:
- Compute the mean face.
- Subtract the mean face from all training images.
- Compute the covariance matrix and its eigenvectors (Eigenfaces).
- Project the training images onto the face space (eigen projections).

### 3. Image Reconstruction

Reconstruct images from the eigen projections and visualize differences for different numbers of principal components.

### 4. Visualize Mean Face

Visualize the mean face (average of all training faces).

### 5. Face Recognition

Implement a face recognition module that:
- Projects test images onto the face space.
- Compares the projected test images to the training images in the face space.
- Computes the recognition accuracy for different numbers of principal components.

## Results

The results section should include:
- Reconstructed images with varying numbers of principal components.
- Visualization of the mean face.
- Recognition accuracy for different numbers of principal components.

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/NithinV-tech/FACE-AGE-PREDICTION.git
   cd FACE-AGE-PREDICTION
