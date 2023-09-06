# Automated Summary Evaluation
Automate the assessment of student-written summaries with a focus on summaries from grades 3-12. Our model evaluates the quality based on representation of main ideas, details from the source text, and the clarity, precision, and fluency of the language.

## Table of Contents
### Project Overview
### How to Use
### Setup
### Extracting Embeddings
### Model Training
### Evaluation


## Project Overview
Context: Summary writing is an essential skill, crucial for enhancing reading comprehension, especially for second language learners and those with learning disabilities. Evaluating these summaries manually is time-intensive, but with the aid of large language models (LLMs) and other tech, this process can be significantly streamlined.

Objective: Develop a model that evaluates student-written summaries. The model's evaluation metrics include the representation of main ideas, the quality of language used in terms of clarity, precision, and fluency.


## How to Use
Setup
Ensure you have Python 3.6 or newer installed.
Install the required libraries:


## Extracting Embeddings
Utilize the get_bert_embedding function available in the main codebase to extract embeddings for any given text.


## Model Training
Split your data into training and test subsets.
Train the model using features derived from BERT.

## Evaluation
The project uses MCRMSE (mean columnwise root mean squared error) as the primary evaluation metric. The objective is to achieve the smallest value possible for this metric.

<br>