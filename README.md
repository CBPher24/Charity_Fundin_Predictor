# Charity_Fundin_Predictor
With knowledge of machine learning and neural networks, I’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.


Report

In this analysis, was looking to try to detemine if could make a prediction on if an application would be successful and worth investing in. Shall breakdown the data and attempt to find a good model that will be able to have an accuracy of over 75%. Shall walk through a little of the data setup now:

1.  Used the data "IS_SUCCESSFUL" as my target since ultimately this is the goal we are going for. If an investment in a charity application is succesful, then it was worh investing in.
2.  Variables I left in the data to be included was APPLICATION_TYPE,  AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
3.  I dropped STATUS completely from the model because whether it is finished or still going it was either successful or not.

![alt text](https://colab.research.google.com/drive/1-Wkm_Sc-sfOJkD5Ido4msZWNJJOF20DS#scrollTo=T8mVEDi10koR)
