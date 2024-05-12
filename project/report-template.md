# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Dina Mostafa Osman

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: i needed to clear the cell's output as the file size was very large, but it failed also so i submited the submissions.csv file only

### What was the top ranked model that performed?
TODO: the model with added new features

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: i found that not all the features has the same distribution and i added new features from datetime column with .dt method

### How much better did your model preform after adding additional features and why do you think that is?
TODO: my score is improved from 1.84672 to .59398 which means the model performed much better

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: my score is improved from .59398 to  .77911 which means the model performes less betetr

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: in Hyper parameter tuning

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|XGBoost_BAG_L2/T4|XGBoost_BAG_L2/T3|ExtraTreesMSE_BAG_L2|score|
|--|--|--|--|--|
|initial|default|default|default|1.84672|
|add_features|default|default|default|0.59398|
|hpo|{'n_estimators': 10000, 'learning_rate': 0.13416642577896967,'n_jobs': -1,'proc.max_category_levels': 100,'objective': 'reg:squarederror', 'booster':'gbtree','max_depth': 3,'min_child_weight': 5,'colsample_bytree': 0.7187936056313462}|{'n_estimators': 10000,'learning_rate':0.02386109712430462,'n_jobs': -1,'proc.max_category_levels': 100,'objective': 'reg:squarederror','booster': 'gbtree','max_depth': 8,'min_child_weight': 3,'colsample_bytree': 0.7724415914984484}|{'n_estimators': 10000,'learning_rate': 0.09276005809908329,'n_jobs': -1,'proc.max_category_levels': 100,'objective': 'reg:squarederror','booster':'gbtree','max_depth':10,'min_child_weight':1,'colsample_bytree':0.6917207594128889}
|0.77911|


### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](https://github.com/DinaMostafa25/cd0385-project-starter/blob/main/project/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](https://github.com/DinaMostafa25/cd0385-project-starter/blob/main/project/model_test_score.png)

## Summary
TODO: Add your explanation
