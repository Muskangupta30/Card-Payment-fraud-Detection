Card Payment Fraud Detection

The aim of this project is to predict fraudulent credit card transactions using machine learning models.

Data Understanding

As you saw, the data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for only 0.172% of the total transactions. The data set has also been modified with principal component analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value of 1 in the cases of fraud and 0 in others.

The distribution plots of the variables were Gaussian, which might indicate the effects of transformations that had already occurred on the data set.

So, when you applied PCA on the data set, the new variables were weighted combinations of the original features.

Project Pipeline

You got an intuitive understanding of the data set and understood the type of data that we have and the distribution of each of the variables in the data set. You saw that owing to the PCA transformation, the final variables obtained were normally distributed.

The project pipeline can be briefly summarised in the following four steps:

Data understanding

Exploratory data analytics (EDA)

Train/Test split

Model building / hyperparameter tuning
