# Metal Surface Defect Classifier

A Convolutional Neural Network (CNN) system for automatically classifying surface defects in steel images using the NEU-CLS dataset.

## Project Overview

This project investigates automated visual inspection of steel surfaces using deep learning. A CNN is trained to identify different types of surface defects from grayscale steel images.

The project includes data preprocessing, CNN training, model evaluation, and an interactive prototype that allows a user to upload a steel surface image and receive a predicted defect class and confidence score.

## Defect Classes

The system classifies six steel surface defect categories:

- Crazing
- Inclusion
- Patches
- Pitted Surface
- Rolled-in Scale
- Scratches

## Dataset

The project uses the NEU-CLS steel surface defect dataset.

The dataset contains 1,800 grayscale images across six defect classes.

The data is divided into:

- Training set: 1,260 images
- Validation set: 270 images
- Test set: 270 images

## Model

The baseline classifier is a Convolutional Neural Network (CNN) developed using PyTorch.

The training pipeline includes:

- Image preprocessing and resizing
- Data augmentation
- CNN feature extraction
- Classification into six defect classes
- Validation during training
- Evaluation on a held-out test set

## Evaluation

Model performance is evaluated using:

- Test accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Training and validation loss/accuracy curves

The trained baseline model achieved approximately **96.3% test accuracy**.

## Working Prototype

An interactive prototype is included in the notebook.

The prototype allows a user to:

1. Upload a steel surface image.
2. Preprocess the image using the same pipeline used during model evaluation.
3. Run the image through the trained CNN.
4. Display the predicted defect class.
5. Display the model confidence.

Example prototype result:

- Uploaded image: `scratches_132.jpg`
- Predicted class: `scratches`
- Confidence: `98.30%`

## How to Run

1. Open the `.ipynb` notebook in Google Colab.
2. Select a GPU runtime if available.
3. Run the notebook cells from top to bottom.
4. Train and evaluate the CNN.
5. Run the interactive prototype cell.
6. Click **Choose Files** and upload a steel surface image.
7. View the predicted defect class and confidence score.

## Technologies

- Python
- PyTorch
- Torchvision
- Google Colab
- NumPy
- Matplotlib
- Scikit-learn
- Pillow

## Repository Contents

- `Task2_Baseline_CNN_SteelDefect (1).ipynb` — CNN training, evaluation, and working prototype
- `README.md` — project documentation

## Project Team

**Group 10**

- Reentseng Mokoena
- Thembelani Mkhulise
- Khulasande Gwamanda
- Balungile Mdlalose
