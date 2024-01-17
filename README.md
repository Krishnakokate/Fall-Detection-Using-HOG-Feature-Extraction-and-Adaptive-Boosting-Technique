# Fall Detection Using HOG Feature Extraction and Adaptive Boosting Technique

## Overview

This project aims to develop a reliable and accurate fall detection system using machine learning techniques. The system utilizes accelerometer and gyroscope measurements, employing the Histogram of Oriented Gradients (HOG) method for feature extraction. Various classification algorithms, including K-nearest neighbors (KNN), decision tree (DT), support vector classifier (SVC), and ensemble learning Boosting, are implemented to enhance accuracy.

## Dataset

The Fall Detection Dataset from Kaggle is used for training and testing. The dataset comprises accelerometer and gyroscope measurements collected from a kaggle  by subjects during activities like walking, standing, sitting, and falling.

## Methodology

1. **Data Collection and Preprocessing:**
   - Video clips of simulated falls and non-falls are processed to extract frames and convert them into grayscale images.
   - Image dataset is cleaned, resized, normalized, and augmented for effective model training.
2. **Exploratory Data Analysis (EDA):**
   - Conducted EDA on the dataset to understand its characteristics and distributions.
3. **Feature Extraction using HOG:**
   - HOG technique is employed to analyze the distribution of edge orientations in each image.
   - Image gradients, magnitude, orientation, histograms, block normalization, and descriptor calculation are performed.

4. **Classification Algorithm (Ensemble Learning Boosting):**
   - Logistic Regression, Decision Tree, SVM Classifier, and KNN are utilized as individual classifiers.
   - Ensemble learning Boosting is applied to combine predictions from multiple classifiers.

5. **Cross-Validation:**
   - Model effectiveness is assessed using cross-validation, calculating accuracy, recall, precision, and F1 score.

6. **Model Evaluation and Results:**
   - Trained models (Decision Tree, Logistic Regression, SVM, KNN, and Adaptive Boosting) are tested and compared using accuracy scores.
   - Confusion matrix is generated to analyze model performance.



## Usage

### Prerequisites
  - Python 3.x
  - numpy
  - pandas
  - matplot
  - seaborn
  - sklearn

1. Clone the repository:

   ```bash
   git clone https://github.com/Krishnakokate/Fall-Detection-Using-HOG-Feature-Extraction-and-Adaptive-Boosting-Technique.git
   cd fall-detection

2. Install dependencies:

   ```bash
   pip install -r requirements.txt


3. Mount Google Drive (if using Colab):

   ```bash
   from google.colab import drive
   drive.mount('/content/drive')
   
5. Define dataset path and configure parameters:

   ```bash
   root_dir = '/content/drive/MyDrive/dataset'
  
6. Run the main script:

   Fall_Detection.ipynb
