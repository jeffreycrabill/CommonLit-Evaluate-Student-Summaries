# CommonLit-Evaluate-Student-Summaries
Automated Summary Evaluation
The goal of this project is to automate the assessment of student-written summaries, ranging from grades 3-12. Our objective is to build a model that evaluates the quality of a summary based on its representation of the main ideas and details from the source text. Additionally, we consider the clarity, precision, and fluency of the language used.

Project Overview
Context
Summary writing is a fundamental skill for learners. It not only enhances reading comprehension but is particularly beneficial for second language learners and those with learning disabilities. With that said, evaluating these summaries manually can be labor-intensive. By leveraging large language models (LLMs) and other technological advancements, we can significantly improve and streamline this evaluation process.

Objective
To develop a model adept at evaluating the quality of student-written summaries. The criteria for evaluation encompass:

Representation of main ideas and details from the source text.
Clarity, precision, and fluency of the language used.
How to Use
Setup
Ensure you have Python 3.6 or newer installed.
Install the required libraries:
bash
Copy code
pip install transformers torch numpy scikit-learn
Extracting Embeddings
Use the get_bert_embedding function provided in the main code to extract embeddings for a given text.
Model Training
Split the data into training and test sets.
Train your model using the features extracted from BERT.
Evaluation
This competition uses the MCRMSE (mean columnwise root mean squared error) for evaluation. The goal is to minimize this metric.

Acknowledgments
This project is part of a competition hosted by CommonLit in collaboration with the Learning Agency Lab, Vanderbilt University, and Georgia State University. We extend our gratitude to the Walton Family Foundation and Schmidt Futures for their support.