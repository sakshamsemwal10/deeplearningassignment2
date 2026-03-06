#  Fashion-MNIST Image Classification using CNN & Transfer Learning

This assignment implements **Convolutional Neural Networks (CNNs)** and **Transfer Learning techniques** to perform **multiclass image classification** on clothing images.

The project uses the **Fashion-MNIST dataset** to train deep learning models capable of identifying clothing categories such as shirts, shoes, bags, and dresses. It demonstrates the effectiveness of both **custom CNN architectures** and **pretrained models (MobileNetV2)** for image classification tasks.

---

#  Project Overview

Image classification is one of the most common tasks in **computer vision and deep learning**. This assignment explores how CNN-based models can automatically learn visual features from images and classify them into multiple categories.

The project workflow includes:

* Image preprocessing
* Data augmentation
* CNN model development
* Transfer learning implementation
* Model training and evaluation
* Performance comparison between models

The goal is to understand how **deep learning models learn visual patterns from image data**.

---

#  Problem Statement

Traditional machine learning algorithms struggle with **image data due to high dimensionality and complex visual patterns**.

Convolutional Neural Networks solve this problem by:

* Automatically extracting hierarchical features from images
* Learning spatial patterns using convolution filters
* Improving classification accuracy with deep architectures

This assignment demonstrates how CNNs and transfer learning can improve **multiclass image classification performance**.

---

#  Dataset Description

The project uses the **Fashion-MNIST dataset**, a widely used benchmark dataset for image classification.

Dataset characteristics:

* **70,000 grayscale images**
* **28 × 28 pixel resolution**
* **10 clothing categories**

Example categories include:

```id="6b4u2v"
T-shirt / Top
Trouser
Pullover
Dress
Coat
Sandal
Shirt
Sneaker
Bag
Ankle Boot
```

Each image is labeled with its corresponding clothing category.

---

#  Image Preprocessing

Before training the models, images undergo several preprocessing steps:

* Normalization of pixel values
* Reshaping images to match CNN input format
* Preparing image tensors for neural network processing

These steps ensure that the dataset is suitable for **deep learning training pipelines**.

---

#  Train–Test Split

The dataset is divided into:

* **Training Set** – used for learning model parameters
* **Testing Set** – used to evaluate model performance on unseen data

This separation ensures that the model's **generalization ability** can be measured accurately.

---

#  Data Augmentation

To increase dataset diversity and reduce overfitting, several **data augmentation techniques** are applied:

* Image rotation
* Zoom transformations
* Width and height shifting
* Horizontal flipping

Data augmentation helps the model become more robust by exposing it to **varied image patterns** during training.

---

#  Custom CNN Architecture

A **custom Convolutional Neural Network (CNN)** is designed to perform image classification.

Model structure:

```id="e8dkn2"
Input Layer (28x28 Image)
        │
        ▼
Convolution Layer
        │
        ▼
Pooling Layer
        │
        ▼
Convolution Layer
        │
        ▼
Pooling Layer
        │
        ▼
Fully Connected Layer
        │
        ▼
Output Layer (Softmax)
```

The convolution layers extract important visual features while pooling layers reduce spatial dimensions.

---

#  Model Compilation

The CNN model is compiled using the following configuration:

| Component         | Method                    |
| ----------------- | ------------------------- |
| Optimizer         | Adam                      |
| Loss Function     | Categorical Cross-Entropy |
| Evaluation Metric | Accuracy                  |

This setup is widely used for **multiclass classification tasks**.

---

#  Model Training

The CNN model is trained on the augmented dataset to learn meaningful image representations.

During training, the network adjusts its weights using **backpropagation and gradient descent** to improve classification performance.

---

#  Training Visualization

To monitor model learning behavior, training graphs are generated:

* **Training Accuracy**
* **Validation Accuracy**
* **Training Loss**
* **Validation Loss**

These visualizations help detect:

* Overfitting
* Underfitting
* Training instability

---

#  Model Evaluation

After training, the model is evaluated using the following performance metrics:

| Metric    | Purpose                                |
| --------- | -------------------------------------- |
| Accuracy  | Overall classification performance     |
| Precision | Correct positive predictions           |
| Recall    | Ability to detect each class correctly |
| F1 Score  | Balance between precision and recall   |

These metrics provide a comprehensive view of model performance.

---

#  Confusion Matrix

A **confusion matrix** is generated to visualize classification performance across all image classes.

```id="m7chx2"
               Predicted Class
              C1 C2 C3 C4 C5 ...
Actual C1      ✔  ✖  ✖
Actual C2      ✖  ✔  ✖
Actual C3      ✖  ✖  ✔
```

This helps analyze which classes are commonly misclassified.

---

#  Transfer Learning

In addition to the custom CNN model, the project uses **Transfer Learning with MobileNetV2**, a pretrained deep learning model.

Transfer learning allows:

* Reusing pretrained feature extractors
* Faster training
* Improved accuracy with limited data

MobileNetV2 is fine-tuned for Fashion-MNIST classification.

---

#  Model Comparison

The project compares two approaches:

1️⃣ **Custom CNN Model**

* Built from scratch
* Learns features directly from the dataset

2️⃣ **Transfer Learning Model (MobileNetV2)**

* Uses pretrained weights
* Faster convergence
* Often achieves higher accuracy

The comparison highlights the benefits of **transfer learning in deep learning workflows**.

---

#  Project Structure

```id="wpl9tv"
├── Assignment2_Report.pdf
├── CNN_Image_Classification.ipynb
└── README.md
```

#  Challenges & Learnings

### CNN Feature Extraction

Understanding how convolution layers detect edges, textures, and patterns was key to building the model.

### Data Augmentation

Augmentation techniques helped improve model generalization and reduce overfitting.

### Transfer Learning

Using pretrained models significantly improved performance while reducing training time.

---

# Author

**Saksham Semwal**

GitHub
https://github.com/sakshamsemwal10

LinkedIn
https://www.linkedin.com/in/saksham-semwal-380220394/

---
