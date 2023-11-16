# Automated Summary Evaluation

## Table of Contents
- [Project Overview](#project-overview)
- [Setup](#setup)
- [How to Use](#how-to-use)
- [Data Preprocessing](#data-preprocessing)
- [Model Training and Architecture](#model-training-and-architecture)
- [Evaluation](#evaluation)
- [Competition Submission](#competition-submission)
- [Troubleshooting and FAQs](#troubleshooting-and-faqs)
- [Contact](#contact)

## Project Overview
This project focuses on automating the assessment of student-written summaries, particularly for grades 3-12. By leveraging advanced technologies like large language models (LLMs), the tool streamlines the evaluation process, which is vital for second language learners and individuals with learning disabilities.

### Objective
To develop a model that evaluates summaries based on the representation of main ideas, clarity, precision, and fluency of language. This automation reduces the time and effort required for manual evaluation.

## Setup
Ensure you have Python 3.6 or newer installed. Download the necessary datasets and organize them as shown from [https://www.kaggle.com/competitions/commonlit-evaluate-student-summaries/data]:
- sample_submission.csv
- prompts_train.csv
- summaries_test.csv
- summaries_train.csv
- prompts_test.csv

Install the required libraries:

pip install numpy pandas tensorflow scikit-learn matplotlib spacy

## How to Use
-Clone the repository and navigate to the project directory.
-Install the required libraries as mentioned above.


## Data Preprocessing
The dataset includes student-written summaries which undergo several preprocessing steps:
- Removing NaN values.
- Text normalization (lowercasing, removing non-alphanumeric characters).
- Stop-word removal using Spacy.

These steps are crucial for cleaning the data and preparing it for vectorization.

## Model Training and Architecture
The project employs a neural network built with TensorFlow and Keras. The architecture includes several Dense layers with activation functions and Dropout for regularization.

**Training Process:**
- Data is split into training and test sets.
- CountVectorizer is used for vectorizing text data.
- The model is trained for 10 epochs with a batch size of 32.

## Evaluation
We use RMSE (Root Mean Squared Error) as the primary metric for evaluating the model's performance. Lower RMSE values indicate better model accuracy in predicting the quality of summaries.

## Competition Submission
For those using this model for competition submissions:
- Format your predictions as specified by the competition guidelines.
- Use the trained model to predict on new, unseen data.

## Troubleshooting and FAQs
If you encounter issues, refer to this section for common problems and their solutions.

## Contact
For queries or contributions, please reach out to [jeffreycrabill@gmail.com].
