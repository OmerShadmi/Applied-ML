# Applied-ML Project: Skip-Gram Model Implementation

## Project Overview

This project implements a **Skip-Gram model** for learning word embeddings using a dataset of hotel reviews. The model is trained to predict context words from a target word, which helps in learning the relationships between words. The implementation follows an efficient and scalable approach to handle large datasets and generate meaningful word embeddings.

The project is structured in a Jupyter notebook and includes functions for data preprocessing, vocabulary creation, training data generation (positive and negative samples), model training, and embedding visualization.

## Dataset

The dataset used in this project consists of **230,339 rows of hotel reviews**. The raw text is processed to remove frequent and rare words to optimize the vocabulary size. The final vocabulary contains approximately **23,000 words**.

## Key Components

### Data Preprocessing:
- Cleaning and tokenizing the text data.
- Creating a vocabulary from the dataset.
- Subsampling frequent words and removing rare ones based on a frequency threshold.

### Training Data Generation:
- Generating positive and negative word pairs using a sliding context window.
- Implementing an efficient negative sampling strategy to generate training data without memory issues.

### Model Architecture:
- **Skip-Gram model** implemented using TensorFlow and Keras.
- The model takes target words and context words as input and trains using negative sampling.

### Word Embeddings:
- After training, the model generates embeddings for words, which can be used for various downstream tasks like word similarity and clustering.

### Visualization:
- Visualization of the word embeddings using dimensionality reduction techniques (e.g., PCA, t-SNE) to explore the relationships between words.

## Usage

### Requirements

- Python 3.10
- TensorFlow 2.12
- Numpy 1.24.4
- Pandas 1.5.3
- Matplotlib 3.8.2
- Seaborn 0.13.2
- Pyarrow
