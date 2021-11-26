# Analaysing-ADHD-dataset
Exploratory data analysis and different machine learning algorithms were applied to the ADHD dataset from the IEEE data port.

# Brief summary
ADHD dataset was considred for this assignment. This dataset consists of two classes ADHD and Control where ADHD means the person is affected with Attention deficit hyperactivity disorder and control means the person is normal.
Each class had mat files where one mat file represents one persons eeg data.These mat files were converted to csv files.Then each csv file which was a 2d matrix which was converted to a vector with average mutual information of every feature which was calculated feature wise.
The labels were also added to these vectors were:-
1 -> ADHD class
0 -> Control class
By finding the minimum mutual information for each feature topoplot was plotted for both the classes.
PCA was performed on the dataset which had 121 rows and 20 columns. The dataset was reduced to a 2 dimensions and was plotted to check if it was linearly separable.The data was not linearly separable.
Then with the help of plotted with explained variance ratio and number of features the optimum number of features for PCA was found. Therefore, for ADHD dataset we require atleast 5 features in order to perform PCA.
Finally the dataset was tested against various machine learning models along with gridsearchcv for hyperparameter tuning. For each model the best results are summarised below :-

Perceptron for classification with accuracy 70%
Logistic Regression with accuracy 64.5%
SVM (different kernels) with accuracy 80%
Naive Bayes a. Benolli Naive Bayes with accuracy 50% b. Gaussian Naive Bayes with accuracy 67.7%
KNN with accuracy 66.6%
Decision Tree with accuracy 73.3%
Random Forest Classifier with accuracy 70.9%

From the above results we can conclude that SVM performed well on ADHD dataset with not only good accuracy but also good precison,recall and F1-score as well
