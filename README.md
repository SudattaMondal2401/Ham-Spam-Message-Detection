# Ham-Spam-Message-Detection

### Introduction 

The following jupyter notebook uses a spam dataset found on kaggle to train ML models that can detect whether a text message or email is a spam or not based on their content.
The link to the dataset can be found [here](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset).

We compare the various ML models available and see which one gives the highest accuracy and f1 score. 

### Uploading the dataset

While uploading the dataset, we had to set our encoding as latin-1, since otherwise we were getting an encoding error.

### Splitting the dataset

Before splitting the dataset, we removed the three unneded columns with a large number of null values.

We also applied the spacy preprocessing to remove the stop words and lemmatize the texts to get more accurate results.

Since there was an unequal number of ham and spam messages, we used stratified split to split the data, so that the ratio of ham to spam in both the training and test set is almost similar.

### Conclusion

Certain models has a high accuracy score but low f1 score (such as K-NN and Decision Tree). We did not choose those models.

According to our work, the top 3 models with the highest accuracy and f1 scores are as follows:
i. Stacking Classifier
ii. SVC (Both Linear and Sigmoid)
iii. Random Forest Classifier

