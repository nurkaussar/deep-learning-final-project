# Project Proposal: Facial Emotion Recognition using Deep Learning

**Student:** Muner Nurkaussar  
**Topic:** Image Classification (Computer Vision)  
**Task:** Recognition of 7 basic human emotions from facial images.

### 1. Problem Statement
The objective of this project is to classify grayscale images of faces into seven basic emotion categories: angry, disgust, fear, happy, sad, surprise, and neutral. This is a classic Computer Vision task with widespread applications in user behavior analysis, security systems, and human-computer interaction interfaces.

### 2. Dataset
The project will utilize the **FER-2013** dataset, a standard benchmark for this task.
* **Source:** Kaggle ([FER-2013 Challenge](https://www.kaggle.com/datasets/msambare/fer2013))
* **Description:** The dataset consists of 35,887 grayscale facial images, each sized 48x48 pixels.
* **Split:** The data is already divided into Training and Testing (PublicTest/PrivateTest) sets.

### 3. Baseline Model
A simple Multi-Layer Perceptron (MLP) or a basic 2-layer Convolutional Neural Network (CNN) will be built as the baseline model. This will establish a minimum accuracy threshold that we will aim to surpass using more advanced deep learning techniques.

### 4. Deep Learning Methodology
To achieve higher accuracy, the following Deep Learning methods will be applied:
* **Architecture:** A deep Convolutional Neural Network (CNN) incorporating `BatchNormalization`, `Dropout` layers to prevent overfitting, and `ReLU` activation functions.
* **Advanced Approach:** Experimentation with Transfer Learning (e.g., adapting pre-trained models like MobileNetV2 or VGG16 for 48x48 input data).
* **Data Augmentation:** Applying random rotations, shifts, and horizontal flips during training to improve the model's generalization capabilities.

### 5. Evaluation Metrics
The model's performance will be evaluated using:
* **Accuracy:** The overall classification accuracy across all classes.
* **Confusion Matrix:** To conduct a detailed error analysis and identify which specific emotions the model confuses most often (e.g., distinguishing between fear and surprise).
* **F1-score:** To evaluate performance on imbalanced classes (e.g., the "disgust" class typically has fewer samples).

### 6. Implementation Plan (Timeline)

| Week | Planned Work | Expected Output |
| :--- | :--- | :--- |
| **Week 1** | Setup repository, Project Proposal, Exploratory Data Analysis (EDA). | Proposal submitted, repository structured, basic data loading script. |
| **Week 2** | Data Preprocessing & Augmentation. Training the Baseline model. | Baseline metrics established and documented. |
| **Week 3** | Building and tuning the main Deep CNN/Transfer Learning model. | Optimized model, saved weights, and training curves (loss/accuracy). |
| **Week 4** | Final evaluation on the test set, Error Analysis, Final Report, and Presentation. | Completed codebase, `final-report.md`, and presentation slides. |
