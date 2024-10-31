# Equivariant Linear Autoencoder for MNIST

This project implements an autoencoder model that is equivariant under horizontal shifts for MNIST images.  For more information see the paper "Geometry of Linear Neural Networks: Equivariance and Invariance under Permutation Groups".

## Project Structure

- **Data Preparation**: The code loads the MNIST dataset, applies random horizontal shifts to the images, and vectorizes them for training.
- **Equivariance Design**: Using a permutation matrix and eigenvector basis, the code constructs a model that maintains equivariance under horizontal shifts.
- **Model Training**: A linear autoencoder for the equivariance design with a reduced-rank representation is trained on the shifted dataset.
- **Evaluation**: The model is evaluated by encoding and decoding random test images to visualize the reconstruction quality. The final errors are presented for both equivariant and non-equivariant autoencoders.

## Requirements

- Python (3.x)
- NumPy
- SciPy
- scikit-learn
- TensorFlow
- Matplotlib

## Usage

1. Install the dependencies.
2. Run the notebook to load the MNIST data, create shifted versions, and train the autoencoder.
3. Visualize the results to see how the autoencoder reconstructs shifted images.

## Goal

This project shows a simple implementation of an equivariant autoencoder that can adapt to horizontal shifts.
