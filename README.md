# Project: Finding Donors for CharityML

This project demonstrates how the income of an individual can be predicted from census data using supervised learning. 
The income prediction is used to determine which individual could be a potential target for funds raising campaign by CharityML, 
which is a fictitious charity organization. The project dataset is a modified U.S. census dataset, which 
consists of 45,222 data points, with each datapoint having 14 features. 
The original dataset is hosted on [UCI](https://archive.ics.uci.edu/ml/datasets/Census+Income).
The modification consist of removing the 'fnlwgt' feature and records with missing or corrupted entries.

The project is a supervised learning model used to predict if an individual earns above $50,000.  

## Model Description

The final model selected for the project is the AdaBoostClassifier from sklearn library in Python. It is an ensemble of 
the DecisionTreeClassifier and is composed of 400 estimators. The greater the number of estimators the better 
the model performs, but the training time also increases. 

Three models were considered for the project, they are: the Naive Bayes classifier, the decision tree model and 
the AdaBoostClassifier. The AdaBoostClassifier model outperformed on the test set, for both accuracy and F-beta score, with 0.5 as beta.
The project includes a grid search for hyperparameter tuning. The best performing model on the test set was tuned to improve
its performance. The final scores for the AdaBoostClassifier are: accuracy equal to 0.8652, and 0.7401 as F-score.
 
The project also has the analysis of feature importance to uncover the top features responsible for positive prediction. 

## Installation

This project requires **Python 3.x** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

## Code

The code is provided in the `finding_donors.ipynb` notebook file.

## Run

In a command window, navigate to the top-level project directory (that contains this README) and 
run the following command (for Windows):

```bash
jupyter notebook finding_donors.ipynb
```

