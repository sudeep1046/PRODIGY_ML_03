# PRODIGY_ML_03

# Cats vs. Dogs Image Classification

This project demonstrates the use of a Support Vector Machine (SVM) classifier to distinguish between images of cats and dogs.

## Table of Contents
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Model Evaluation](#model-evaluation)
- [Visualization](#visualization)
- [Acknowledgements](#acknowledgements)

## Dataset
The dataset used in this project is the "Cats and Dogs" dataset from Kaggle, which includes images of cats and dogs divided into training and testing sets.

## Requirements
- Python 3.6+
- pandas
- numpy
- scikit-learn
- tensorflow
- keras
- scikit-image
- matplotlib

## Installation
Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/your-username/cats-vs-dogs.git
cd cats-vs-dogs
```

Install the required packages:

```bash
pip install pandas numpy scikit-learn tensorflow keras scikit-image matplotlib
```

## Usage

### Kaggle API Setup
Ensure you have your Kaggle API key (`kaggle.json`) and place it in the appropriate directory.

### Dataset Download
Download the dataset from Kaggle and unzip it:

```bash
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle
!kaggle datasets download -d stefancomanita/cats-and-dogs-40
!unzip cats-and-dogs-40.zip -d /content
```

### Feature Extraction
The images are resized to 40x40 pixels and flattened for input into the SVM classifier.

### Training
Split the data into training and testing sets, and train the SVM classifier using GridSearchCV for hyperparameter tuning.

### Testing
Evaluate the model on the test set and visualize the results.

### Running the Code
Execute the code to train the model and visualize predictions:

```python
python classify_cats_dogs.py
```

## Model Evaluation
The model achieves an accuracy of 62.5%. The classification report provides precision, recall, and f1-score for both classes.

## Visualization
Visualize sample predictions using matplotlib to see how well the model classifies new images.

## Acknowledgements
- The dataset source for "Cats and Dogs" from Kaggle.
- The scikit-learn, pandas, tensorflow, keras, scikit-image, and matplotlib teams for their amazing libraries.

