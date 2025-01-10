# Text Classification using LLMs

## Project Overview
In this project, we aimed to develop advanced models for text classification, specifically binary sentiment classification for movie reviews. The reviews were categorized into two classes:
- **Positive (1)**
- **Negative (0)**

For each review, an identifier and the text were provided. Using the training data (`train.csv`), we trained our models and made predictions on the test data (`test.csv`).

---

## Datasets
We utilized several files for the project:

- **`train.csv`**: Contains the training data with the following columns:
  - `id`: Unique identifier for each review
  - `label`: Sentiment label (1 for positive, 0 for negative)
  - `text`: The review text

- **`test.csv`**: Contains the test data with the following columns:
  - `id`: Unique identifier for each review
  - `text`: The review text

- **`vocab.txt`**: The valid vocabulary for the dataset (one word per line).

- **`sample.csv`**: A sample submission file formatted as:
  - `id`: Review identifier
  - `label`: Predicted sentiment label

---

## Approach and Implementation
1. **Pre-trained Models**:
   We explored multiple pre-trained language models and fine-tuned them for the sentiment analysis task. The models included:
   - **BERT**
   - **DISTIL-BERT**
   - **ROBERTA**
   - **ROBERTA LARGE**

   Among these, **ROBERTA LARGE** achieved the highest accuracy on both the training and test datasets.

2. **Hyperparameter Tuning**:
   We experimented with various hyperparameters to optimize the model performance, including:
   - Learning rate
   - Number of epochs
   - Batch size

   **Key findings**:
   - Increasing the number of epochs beyond 5 or 6 yielded minimal improvement.
   - Increasing the batch size beyond 16 showed diminishing returns.

3. **Model Evaluation**:
   By combining different pre-trained models and hyperparameter configurations, we trained nearly 20 models. From these, we submitted predictions from 9 models, achieving test set accuracy in the range of **87% to 95%**.

---

## Conclusion
Through the application of advanced language models and extensive hyperparameter tuning, we were able to:

- Identify **ROBERTA LARGE** as the best-performing model for this dataset.
- Understand the impact of various hyperparameter settings on model performance.
- Achieve a high level of accuracy (up to **95%**) in sentiment classification for movie reviews.
