# Charity_Fundin_Predictor
With knowledge of machine learning and neural networks, I’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.


Report

In this analysis, was looking to try to detemine if could make a prediction on if an application would be successful and worth investing in. Shall breakdown the data and attempt to find a good model that will be able to have an accuracy of over 75%. Shall walk through a little of the data setup now:

1.  Used the data "IS_SUCCESSFUL" as my target since ultimately this is the goal we are going for. If an investment in a charity application is succesful, then it was worh investing in.
2.  Variables I left in the data to be included was APPLICATION_TYPE,  AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
3.  I dropped STATUS completely from the model because whether it is finished or still going it was either successful or not.

I first set the model to have 2 hidden layers both activating with Relu the first having 8 neurons and the second with 5 follow by the output activating sigmoid. Felt this was a pretty basic setup to start with to begin working off of, choosing sigmoid as the output because the end result is a binary decision being the investment was successful or not.
I then played with multiple setting doing just quick tests to see how they started off but ended up going with adding more Classification and Application types instead of having a large numbered lumped in one variable along with lowering the number of neurons in the 2nd layer.
My second optimization I went back to my initial data set and model but changed all the activation types to sigmoid. Felt because almost all the data was binary it could produce a better result.
My last optimization I combined both of the previous optimizations along with adding a 3rd layer. So the ending model had 3 hidden layers and a output layer; all of which were activating with sigmoid and the neurons went in order of 8, 4 and 2 in the hidden layers.

The end result was I was not able to achieve the desired accuracy results. The best I got was a 72.6% accuracy rate which was with the second optimization. I would have to spend a lengthy amount of time conducting multiple experiments to get a the desired results. I did notice that even the littlest thing plays its part but with large data sets its hard to find the best optimization and I would probably let the keras tuner run multiple experiments to find the best model.