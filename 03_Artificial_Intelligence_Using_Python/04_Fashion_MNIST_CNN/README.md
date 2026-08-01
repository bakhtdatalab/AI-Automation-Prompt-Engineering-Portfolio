# Fashion-MNIST Image Classification Using CNN

## Project Overview

This project focuses on building and evaluating a **Convolutional Neural Network (CNN)** to classify clothing images from the Fashion-MNIST dataset.

The project demonstrates a complete deep-learning workflow, including:

- Loading an image dataset
- Preprocessing image data
- Normalizing pixel values
- Reshaping images for CNN input
- Designing a CNN architecture
- Training the model
- Evaluating model performance
- Generating predictions
- Visualizing results

The model learns to identify different categories of clothing from grayscale images.

## Dataset

**Dataset:** Fashion-MNIST

Fashion-MNIST is a dataset of grayscale clothing images used for image-classification tasks.

Each image represents one clothing category, such as:

- T-shirt or top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle boot

The images are used to train and evaluate the CNN model.

## Project Objectives

The main objectives of this project were to:

- Load the Fashion-MNIST dataset.
- Explore the training and test data.
- Normalize image pixel values.
- Reshape images for CNN input.
- Display sample images and their labels.
- Design a Convolutional Neural Network.
- Train the model using training data.
- Validate the model during training.
- Evaluate the model using unseen test data.
- Generate image-classification predictions.
- Analyze model performance using classification metrics and visualizations.

## Project Workflow

```text
Fashion-MNIST Dataset
          ↓
Image Exploration
          ↓
Pixel Normalization
          ↓
Image Reshaping
          ↓
CNN Model Design
          ↓
Model Training
          ↓
Validation
          ↓
Test Evaluation
          ↓
Image Classification
          ↓
Performance Analysis
```

## Data Preprocessing

### 1. Dataset Loading

The Fashion-MNIST training and test datasets were loaded using TensorFlow/Keras.

The dataset was divided into:

- **Training Data** — Used to train the CNN model.
- **Test Data** — Used to evaluate the model using unseen images.

### 2. Pixel Normalization

Image pixel values were normalized to the range:

```text
0 to 1
```

Normalization helps the neural network process the image data more efficiently and supports stable model training.

### 3. Image Reshaping

The grayscale images were reshaped to include a channel dimension required by the CNN.

The image structure was prepared in the following format:

```text
Height × Width × Channels
```

For grayscale images:

```text
28 × 28 × 1
```

### 4. Image Visualization

Sample images and their corresponding labels were displayed to verify the dataset and understand the clothing categories.

## CNN Model Architecture

The Convolutional Neural Network includes the following types of layers:

- Convolutional layers
- MaxPooling layers
- Dropout layers
- Flatten layer
- Dense layers
- Output classification layer

### Convolutional Layers

Convolutional layers automatically learn important visual features from the images, such as:

- Edges
- Shapes
- Patterns
- Clothing features

### MaxPooling Layers

MaxPooling reduces the spatial size of feature maps while retaining important information.

### Dropout Layers

Dropout helps reduce overfitting by randomly disabling some neurons during training.

### Flatten Layer

The Flatten layer converts the learned image features into a one-dimensional format.

### Dense Layers

Dense layers combine the learned features and support the final classification process.

### Output Layer

The output layer predicts the probability that an image belongs to each clothing category.

## Model Training

The CNN model was trained using the Fashion-MNIST training dataset.

A validation split was used to monitor model performance during training.

The training process was used to observe:

- Training accuracy
- Validation accuracy
- Training loss
- Validation loss

## Model Evaluation

The trained model was evaluated using unseen test images.

The following evaluation methods were used:

- Test accuracy
- Test loss
- Confusion matrix
- Classification report

### Confusion Matrix

The confusion matrix was used to compare:

- Actual clothing labels
- Predicted clothing labels

This helps identify which categories were classified correctly and which categories were confused by the model.

### Classification Report

The classification report provides performance metrics such as:

- Precision
- Recall
- F1-score
- Support

## Model Performance Visualizations

The project includes visualizations for:

- Training accuracy
- Validation accuracy
- Training loss
- Validation loss

These visualizations help evaluate the learning behavior of the model and identify possible overfitting or underfitting.

## Prediction Results

The trained CNN model was used to predict clothing categories for test images.

Sample images were displayed with:

- Actual label
- Predicted label

This provides a visual comparison between the correct category and the model's prediction.

## Tools and Technologies

- Python
- Google Colab
- Jupyter Notebook
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn

## Deep Learning Concepts Demonstrated

- Deep Learning
- Computer Vision
- Image Classification
- Convolutional Neural Networks
- Convolutional Layers
- MaxPooling
- Dropout
- Neural Network Training
- Model Validation
- Multi-Class Classification
- Model Evaluation

## Skills Demonstrated

- Image-data preprocessing
- Pixel normalization
- Image reshaping
- CNN model design
- Deep-learning model training
- Model validation
- Image classification
- Prediction generation
- Classification evaluation
- Confusion-matrix analysis
- Performance visualization

## Project Files

```text
04_Fashion_MNIST_CNN/
│
├── README.md
├── fashion_mnist_cnn.ipynb
└── fashion_mnist_cnn.pdf
```

## File Descriptions

### Jupyter Notebook (`.ipynb`)

The Jupyter Notebook contains:

- Python code
- Dataset loading
- Image preprocessing
- CNN model development
- Model training
- Validation results
- Test evaluation
- Classification outputs
- Performance visualizations

### PDF (`.pdf`)

The PDF contains:

- The completed exercise documentation
- Screenshots of the Python code
- Screenshots of model outputs
- Training and evaluation results
- Evidence of the completed deep-learning tasks

## Learning Outcomes

Through this project, I developed practical experience in:

- Working with image datasets.
- Preparing image data for deep-learning models.
- Normalizing pixel values.
- Reshaping images for CNN input.
- Designing a Convolutional Neural Network.
- Training and validating a deep-learning model.
- Evaluating a multi-class classification model.
- Interpreting classification metrics.
- Analyzing a confusion matrix.
- Visualizing model accuracy and loss.
- Generating predictions for unseen images.

## Future Improvements

Possible improvements include:

- Testing different CNN architectures.
- Adjusting the number of convolutional filters.
- Experimenting with different dropout rates.
- Applying data augmentation.
- Tuning training parameters.
- Using early stopping.
- Testing additional optimization algorithms.
- Comparing the CNN with other image-classification models.
- Deploying the trained model as an interactive web application.

## Author

**Bakht Zamin**

AI Automation & Prompt Engineering | Data Analytics & Business Intelligence | Python | Machine Learning

---

*This project was completed as part of the Artificial Intelligence Using Python course.*
