# Cat DCGAN Project

This repository contains the implementation of a Deep Convolutional Generative Adversarial Network (DCGAN) for generating images of cats. The project consists of three main components:
1. **DCGAN Notebook**: The main implementation of the DCGAN architecture.
2. **Preprocessing Script**: A Python script for preprocessing the cat image dataset.
3. **Trained Model**: An H5 file containing the trained generator model.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [File Descriptions](#file-descriptions)
- [Acknowledgements](#acknowledgements)

## Overview
The goal of this project is to generate realistic images of cats using a DCGAN. The project demonstrates the power of generative models and serves as a proof of concept for generative AI.

## Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/cat-dcgan.git
    cd cat-dcgan
    ```
## Usage
### Training the DCGAN
1. Ensure you have a dataset of cat images larger than 128x128 pixels.
2. Run the preprocessing script to prepare the dataset:
    ```bash
    python preprocessing_cat_dataset.py --data_dir path/to/your/dataset
    ```
3. Train the DCGAN by running the Jupyter notebook `DCGAN.ipynb` or the equivalent Python script.

### Generating Cat Images
After training, you can use the trained model to generate cat images. Load the model from the `cat_generator_model-250epochs.h5` file and use it to generate new images.

## File Descriptions
- **DCGAN.ipynb**: The main implementation of the DCGAN architecture.
- **preprocessing_cat_dataset.py**: Script for preprocessing the cat image dataset.
- **cat_generator_model-250epochs.h5**: Trained generator model saved after 250 epochs.

### DCGAN Notebook
The notebook contains the following sections:
1. **Generator Architecture**: Defines the architecture of the generator model.
2. **Discriminator Architecture**: Defines the architecture of the discriminator model.
3. **Loss Functions**: Defines the loss functions for the generator and discriminator.
4. **Training Loop**: Contains the training loop for training the DCGAN.
5. **Data Preprocessing**: Prepares the cat image dataset for training.
6. **Model Training**: Trains the DCGAN and saves the generator model.

### Preprocessing Script
The preprocessing script resizes and augments the images to prepare them for training. It also generates a DataFrame for use with the Keras ImageDataGenerator.

### Trained Model
The trained generator model can be loaded and used to generate new images of cats.

## Acknowledgements
This project was inspired by the original DCGAN paper by Radford, Metz, and Chintala. Special thanks to the TensorFlow and Keras teams for their excellent libraries.
