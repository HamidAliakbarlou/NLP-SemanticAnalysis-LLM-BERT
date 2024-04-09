# Text Classification using LLMs

In this project, we want to try to develop advanced models for text classification.
The goal is to do binary sentiment classification for each movie review. The reviews are classified into two categories (positive 1, negative - 0). For each review, we receive an identifier and the text. We would work on the training data (train.csv), and then make the predictions for the test data (test.csv).

### Datasets
We have several data files for the project

• train.csv: the training texts (id, label, text)

• test.csv: the test texts (id, text)

• vocab.txt - the valid vocabulary for the dataset (word)

• sample.csv: a sample submission file in the correct format (id, label)

### Conclusion on my contribution and findings
1- We investigated multiple pre-trained models with a vast corpus and fine-tuned them for the sentiment analysis task (binary classification) of the dataset we were given. We tried BERT, DISTIL-BERT, ROBERTA, and ROBERTA LARGE. By using ROBERTA LARGE we achieved the highest accuracy for both model and also test set.

2- We also tried to work on tuning the hyperparameters. We played with learning rate, #epochs, and batch size to see how they affect the model performance! We tested multiple combinations of them and finally, It turned out that an epoch more than 5 or 6, is no longer much helpful. This was the same when increasing batch size after 16.

3- Finally considering different pre-trained models and different combinations of hyperparameters tuning, we achieved close to 20 different models out of which We submitted 9 of them which resulted in achieving accuracy on the test set in the range of 87%, up to 95%.
