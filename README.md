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

Challenges
a) Imbalanced Datasets: Datasets with unequal quality and quantity result from the rarity of fraudulent activity in comparison to those that are legal. This may have an impact on the model's precision in identifying fraud.
b) Feature engineering: Effective fraud detection depends on selecting the appropriate features. It's difficult to pinpoint the characteristics that most strongly point to fraudulent activity.
c) Data Quality and Quantity: Adaptability to Unique Patterns: Con artists are always changing and coming up with new methods. Conventional models might find it difficult to keep up with new trends in fraud.
d) Minimal Latency Conditions: Processing data in real time is frequently necessary for financial transactions. It can be difficult to create models that can decide quickly without harming accuracy.
e) Privacy issues: Effective fraud detection is necessary, but it can be difficult to strike a balance with data privacy laws. Making sure that laws like the GDPR and others are followed is essential.
f) Updating the Model: Dynamic and continuously learning fraud detection models are required. Model effectiveness must be maintained by periodically retraining and updating them with new data.

Evaluation
The analysis done to calculate the card fraud detection was successfully done and hence it was concluded that based on the given result, the Logistic Regression model with SMOTE stands out as a trustworthy and effective option for fraud detection. High accuracy, sensitivity, specificity, and F1-Score are just a few of the balanced performance metrics that the model demonstrates on both the training and test sets. This shows that the model can distinguish between fraudulent and non-fraudulent transactions with accuracy. The addition of SMOTE improves the model's overall predictive accuracy by strengthening its ability to identify patterns in the minority class. Because of its intrinsic interpretability, Logistic Regression offers transparency in comprehending the impact of individual features on fraud predictions, which promotes confidence in the model's conclusions. In addition, the computational efficiency of the model makes it a viable solution for real-time applications.
