# Sign-Langauge
Original dataset is taken from kaggle - https://www.kaggle.com/datasets/pathikreet/indian
It has been comprised to a smaller version to upload in github

The first step after importing is preprocessing the image dataset is converted to text dataset either into pickle or csv file which reduces the load on model while training.
It is done so by taking 21 points in each hand using mediapipe module and storing the values of each axes for each points.

Then the model is trained on the dataset using RandomeForestClassifier from scikit-learn library . 

Later using OpenCV real time hand detection is done along with capturing points in hand and giving to the model to predict the value.
