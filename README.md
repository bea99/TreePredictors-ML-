The aim of this project is the implementation from scratch of tree predictors for binary classification, to determine whether mushrooms are poisonous. 

The project starts with the definition of classes for the internal nodes and for tree predictors themselves.
After having analyzed the dataset, transforming all the categorical variables into numerical ones using One-hot encoding, it has been divided into training and test set to apply the algorithms.
The tree predictors have been trained according to the classes, adopting two stopping criteria (maximum tree depth and minimum number of splits), whose optimal values have been found given a specific range, and three criteria for the expansion of the leaves (Gini, Entropy and Squared Error).

Since evaluating the model on the whole dataset does not conduct to a good approximation, a way to improve is applying hyperparameter tuning, using RandomizedSearchCV, according to the splitting criteria and the stopping criteria previously adopted. 

The next step is the implementation of Random Forest classifier by reusing the already implemented tree predictor structure, so that the building of several independent trees leads to a more robust model.

The models have been evaluated through cross-validation scores and validation curves.
