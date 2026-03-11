# Rice Leaf Disease Classification using Vision Transformer (ViT)

## Overview

Rice is one of the most important food crops worldwide, and early identification of plant diseases is essential for maintaining crop health and improving yield. Manual disease detection is time-consuming and requires agricultural expertise.

This project explores a deep learning approach for automatically classifying rice leaf diseases using the **Vision Transformer (ViT)** architecture. The model learns visual patterns from rice leaf images and predicts the disease category.

The project also investigates model performance under different classification setups, including **3-class and 5-class disease classification**.

---

## Project Objectives

* Build an automated system for rice leaf disease classification.
* Train a **Vision Transformer (ViT)** model on rice leaf image datasets.
* Compare performance across different classification setups.
* Improve learning on imbalanced datasets using **Class-Balanced Focal Loss**.
* Evaluate model predictions using separate inference notebooks.

---

## Dataset

The dataset contains images of rice leaves affected by different diseases. Each image belongs to a specific disease category.

Two classification setups are explored in this project:

### 3-Class Classification

A simplified dataset with three disease categories.

### 5-Class Classification

A more detailed dataset with five disease categories.

Images are preprocessed and resized before training to maintain consistent input dimensions for the model.

---

## Model Architecture

This project uses the **Vision Transformer (ViT)** model.

Unlike traditional Convolutional Neural Networks (CNNs), Vision Transformers divide an image into patches and process them as sequences using **self-attention mechanisms**. This enables the model to capture global relationships across the entire image.

The model is initialized with pretrained weights and fine-tuned on the rice leaf dataset.

---

## Handling Class Imbalance

To address class imbalance in the dataset, the training pipeline incorporates:

**Class-Balanced Focal Loss**

This loss function adjusts the contribution of each class based on the number of samples, helping the model focus on underrepresented disease categories.

---

## Repository Structure

```
Rice-Leaf-Disease-Classification-ViT
│
├── notebooks
│   ├── 3_class_dataset_training.ipynb
│   ├── 3_class_output.ipynb
│   ├── 5_class_dataset_training.ipynb
│   ├── 5_class_output.ipynb
│   └── combined_dataset_training.ipynb
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Notebook Description

### 3_class_dataset_training.ipynb

Trains a Vision Transformer model on the 3-class rice leaf disease dataset.

### 3_class_output.ipynb

Loads the trained 3-class model and performs predictions on test images.

### 5_class_dataset_training.ipynb

Trains the Vision Transformer model on the 5-class dataset with class imbalance handling.

### 5_class_output.ipynb

Runs inference using the trained 5-class model.

### combined_dataset_training.ipynb

Trains a model using the combined dataset to evaluate performance across merged disease classes.

---

## Installation

Clone the repository:

```
git clone https://github.com/yourusername/Rice-Leaf-Disease-Classification-ViT.git
```

Navigate to the project directory:

```
cd Rice-Leaf-Disease-Classification-ViT
```

Install the required dependencies:

```
pip install -r requirements.txt
```

---

## Running the Project

Open the notebooks using **Jupyter Notebook** or **Google Colab**.

```
jupyter notebook
```

Run the training notebooks to train the model and the output notebooks to perform predictions.

---

## Technologies Used

* Python
* PyTorch
* Vision Transformer (ViT)
* NumPy
* OpenCV
* Scikit-learn
* Matplotlib

---

## Future Improvements

* Training on larger and more diverse rice disease datasets
* Deploying the model as a real-time disease detection tool
* Integrating the model into mobile or web applications for agricultural use
* Improving model explainability using advanced visualization techniques

---

## Author

Varunn M
Hari Prasath J
Pamarthi Sai Narasimham
