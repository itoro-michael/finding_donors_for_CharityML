# Finding Donors for CharityML

Finding Donors for CharityML is one of the required projects, to obtain the Data Scientist Nanodegree from Udacity. 
The project is a supervised learner to predict if an individual earns above a certain amount, which is $50,000.  

## Model Description
[p1_charityml](https://github.com/itoro-michael/finding_donors_for_CharityML/tree/master/p1_charityml)

The final model selected for the project is an ensemble of the decision tree classifier, 
provided by the sklearn library in Python. The ensemble model is composed of 400 weak decision tree classifiers. 
The greater the number of weak classifiers the better the model performs, ultimately the number of classifiers will be 
contrained by the acceptable training time. 

Three models were considered for the project, they are: the Naive Bayes classifier, the single decision tree model and 
the ensemble. The ensemble model outperformed the rest on test set evaluation, for both accuracy and F-score, with beta=0.5. 

The project includes a grid search to determine the optimal number of weak classifiers to adopt, as a hyperparameter. 
Also, there is feature importance analysis to discover the top features responsible for a positive prediction. 