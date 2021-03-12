# Kaggle categorical feature competition

In this kaggle competition there are only ordinal and categorical features in the data frame. The dataset is available at [kaggle categorical feature encoding challange](https://www.kaggle.com/c/cat-in-the-dat).

In the Classifier_and_encoders.ipynb notebook I used different encoding techniques like label encoding, one-hot encoding and count encoding. The models in Classifier_and_encoders.ipynb notebook are regressor models. This needs to be changed to classifier models before applying it on test data and participate in the competition. As I promarily wanted to calculate the probability of y being a cat or not a cat, I used a regressor. A better way is to use a classifier and calculate proba_ feature of the model as one of my other repositories in which I manually made a soft voting ensemble method for inference.

**Note: In the notebook I have kept some of the errors raised by applying different encoders or different algorithms applying on datasets that required more cleaning. All these cells are followed by explaining the problem and a solution to resolve the error.**

In this notebook I showed the power and weaknesses of each encoding, and the challenges of each method. Also I standardized how encoding techniques need to be applied on both train and test data in the right way and to handle unseen values in test data. To resolve this issue I always concatinate train and test data, and later apply the encoder to fit_transform. This way I am sure that both test and train are transformed with the same encoder whle the problem of handling unseen values in test data set is prevented.
