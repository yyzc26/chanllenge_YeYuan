# chanllenge_YeYuan
Hello! This is the challenge I completed for the credit card default project

It is completed using Jupyter notebook following the guidiance

o Data Visualization/Exploration

o Implemented data pre-processing steps
  Created dummy variables for categorical variables(X2, X3, X4)
  Tried under sampling and over sampling to pre-process the data
  
o Explored models that are appropriate for this use case
o Fit selected model to the analytics ready dataset. List outcomes from model fitting
  I picked 'LogisticRegression','DecisionTreeClassifier','RandomForestClassifier','AdaBoostClassifier','GradientBoostingClassifier' to explore based on experience. Due to the time limitation, I didnot try other methods, such as ANN. 
  
o Evaluate model performance on held-out/testing dataset
    20% data are held-out for test.  F1 scores of 0.86 on test data achieved by 'RandomForestClassifier' with over-sampling
    
o What other options would you’ve considered (in solving the problem), if you had additional time?

    I spent a evening on this project (around 3 hr) 
    1, The parameters for these five models are not optimized yet.  
        Gridsearch takes too long on my machine. So I only grid search a few parameters for random forest.  Adaboost and GDBT are also             promissing.  
    2, I also could try ANN
