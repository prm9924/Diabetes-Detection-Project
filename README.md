This project aims to predict diabetes within patients, taking into consideration binary and multi-class classification as well as the effect of balanced and unbalanced classes on prediction power. Take a look at our interactive python notebook (ipynb) file for our code as well as our final paper for a write up of our entire study.

**Abstract**

Diabetes is one of the most common diseases in the world and is especially a major problem in the United
States. This disease affects the body’s ability to break down sugars, glucose in particular, in the blood.
Glucose is an important source of energy for the cells that make up the muscles and tissues. It's also the
brain's main source of fuel. Whether genetically developed or not, the main cause of diabetes varies by type.
But no matter the type of diabetes, when the body loses the ability to break down blood sugar, large amounts
build-up and remain in the bloodstream. Excessive amounts can lead to serious health issues such as heart
disease and kidney failure.

This project evaluates various classical Machine Learning methods as well as a Deep Learning model in
their ability to classify patients as non-diabetic, pre-diabetic, or diabetic. This is based on survey responses
asking participants for measures of blood pressure, cholesterol, general health, and other factors which are
used as predictors in building a classification model. We first use unsupervised learning methods to explore
patterns in our data, with the main goal of reducing dimensionality through PCA and applying clustering
algorithms to see if the diabetes target variable classes are well separated by the clusters. We also study
multicollinearity and regularization for feature importance and selection. Then, we proceed with predictive
modeling and find that tree-based methods like XGBoost as well as the supervised learning method Support
Vector Machine outperform many other models. Our primary means of model evaluation is not only
accuracy, but more so false negative rate. Since our data has severe class imbalances, as the vast majority
of the individuals are non-diabetic Class 0, the model will mostly predict 0 and therefore have a high
accuracy since most test observations will also be Class 0. Further examination shows us that the
performance on predicting the minority class, diabetic individuals, is poor as we find high false negative
rates. This means that patients will be told they do not have when they actually do, which is particularly
concerning. As a result, we place a heavy focus on decreasing this false negative rate. 
