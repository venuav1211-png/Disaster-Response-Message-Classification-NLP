# Disaster-Response-Message-Classification-NLP

## Project Overview

Disasters such as floods, earthquakes, hurricanes, and other emergencies generate thousands of social media messages. These messages contain important information about emergency situations, requests for assistance, infrastructure damage, and public safety.

Manually analyzing these messages can be time-consuming during critical situations.

This project uses **Natural Language Processing (NLP) and Machine Learning** techniques to classify disaster-related social media messages into meaningful categories. It aims to help identify relevant information from large volumes of messages and support disaster response activities.

## Objectives

- Load and explore the HumAID disaster-related dataset.
- Understand message content and category distribution.
- Perform text cleaning and preprocessing.
- Convert textual data into numerical features using TF-IDF.
- Train and compare multiple machine learning classification models.
- Evaluate model performance using classification metrics.
- Build an interactive Gradio application for message classification.

## Dataset

**Dataset Name:** HumAID Dataset

**Source:** QCRI/HumAID-all (Hugging Face)

The dataset contains disaster-related social media messages annotated with different disaster information categories.

Dataset loading is performed using the Hugging Face `datasets` library.

## Technologies and Libraries Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-learn
- Hugging Face Datasets
- TF-IDF Vectorizer
- Joblib
- Gradio

## Project Workflow

### 1. Business Understanding and Problem Statement
Understanding the importance of classifying disaster-related messages and identifying how NLP can support emergency response.

### 2. Data Loading and Exploratory Data Analysis
- Load the HumAID dataset.
- Examine dataset structure and columns.
- Identify missing values and duplicate records.
- Analyze the distribution of message categories.
- Explore message length patterns.

### 3. Text Preprocessing
- Convert text into lowercase.
- Remove URLs and unnecessary characters.
- Remove social media mentions.
- Clean extra spaces.
- Prepare text for feature extraction.

### 4. Feature Extraction
TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert text messages into numerical representations.

Configuration:
- Maximum features: 10,000
- N-gram range: (1, 2)

### 5. Model Building
The following machine learning algorithms are implemented and compared:

1. Multinomial Naive Bayes
2. Logistic Regression
3. Linear Support Vector Machine (Linear SVM)

### 6. Model Evaluation
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Classification Report
- Confusion Matrix

### 7. Model Saving and Gradio Deployment
The trained model and TF-IDF vectorizer are saved using Joblib and used in an interactive Gradio application for message classification.

### 8. Testing the Application
Users can enter disaster-related messages and receive the predicted category through the Gradio interface.

## Installation

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk joblib gradio datasets
```

## How to Run the Project

1. Clone or download this repository.
2. Open the Jupyter Notebook.
3. Install the required dependencies.
4. Run the notebook cells sequentially.
5. Load the dataset and perform preprocessing.
6. Train and evaluate the classification models.
7. Save the selected model and vectorizer.
8. Launch the Gradio application.

## Learning Outcomes

Through this project, I gained practical experience in:

- Understanding real-world NLP problems.
- Working with social media text data.
- Performing text preprocessing.
- Implementing TF-IDF feature extraction.
- Training multiple machine learning classifiers.
- Evaluating classification models.
- Saving trained models using Joblib.
- Deploying an interactive application using Gradio.

## Conclusion

This project demonstrates how NLP and machine learning can be applied to disaster-related social media messages to automatically identify meaningful information.

It provided hands-on experience with the complete NLP and machine learning workflow, from dataset exploration and text preprocessing to model evaluation and application deployment.

**Project Type:** Natural Language Processing | Machine Learning | Text Classification

**Developed using:** Python and Jupyter Notebook
