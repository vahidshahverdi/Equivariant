# Equivariant Linear Autoencoder for MNIST

This repository provides code and data to reproduce the results from our paper: 

**Paper Title**: *Geometry of Linear Neural Networks: Equivariance and Invariance under Permutation Groups*  
**Authors**: [Kathlén Kohn, Anna-Laura Sattelberger, Vahid Shahverdi]

## Purpose

This repository is intended to ensure reproducibility of the results provided in the paper. All code and data provided here allow readers to recreate the main findings, following the SIAM Journal on Matrix Analysis and Applications (SIMAX) standards.

## Project Structure

 **Code File**: The Jupyter notebook is necessary to run the model, perform data preprocessing, and reproduce figures from the paper.


## Reproducing the Results

### Requirements

After loading the required packages, everything should work smoothly.

- **Programming Language**: Python, version 3.10.5
- **Libraries**: 
NumPy version: 1.23.5
SciPy version: 1.9.3
Matplotlib version: 3.6.2
Scikit-learn version: 1.1.3
TensorFlow version: 2.11.0

### Steps to Reproduce

1. **Install Dependencies**: Install the required libraries using `pip install -r requirements.txt`.
2. **Data Preparation**: The MNIST dataset, consisting of 60,000 training and 10,000 test images of handwritten digits (0-9), is loaded directly using TensorFlow's built-in `keras.datasets` module. Each image is grayscale, sized at 28x28 pixels.
3. **Model Training**: Execute the Jupyter notebook `Equivariant_Linear_Autoencoder.ipynb` to train linear autoencoder, semi-equivariant linear autoencoder (without enforcing the realization format from our paper), and linear equivariant autoencdoer. The rank is set at 99 and the group action is the horizontal shift.
4. **Evaluation and Visualization**: Follow the instructions in the notebook to visualize and evaluate the reconstruction quality of shifted images.

### Parameter Settings

All parameter settings used in the experiments are provided in the notebook to facilitate precise reproduction of results. These include training parameters such as batch size, epochs, and network architecture settings.

## Repository Link

The latest version of the code is hosted on a public repository to ensure accessibility: [https://github.com/vahidshahverdi/Equivariant.git].

## Additional Information

For long-term accessibility, a zipped snapshot of this repository will be deposited in SIMAX Supplementary Materials.


