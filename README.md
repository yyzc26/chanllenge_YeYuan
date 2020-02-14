Hello! 

This is the challenge I completed for the credit card default project. 

It is completed following the guidiance

o Data Visualization/Exploration

o Implemented data pre-processing steps.
  1. Normalize numerical columns to [0,1]
  2. Created dummy variables for categorical variables(X2, X3, X4).   
  3. Tried under sampling and over sampling to pre-process the data.(Could have try oversample and undersample together if have more time)
  4. columns X6-X11 are [-2,8], the meaning of these numbers are not very clear. Could do more feature engineering if I can get a deeper understanding on them.  Now they are treated as continous numerical variable, but I fill it may make more sense to treat them categorically
  
o Explored models that are appropriate for this use case.
  The task is too estimate the probability of default. Not a pure binary classification problem.  But I still first implement binary classification to test undersampling and oversampling, and get some metrics.  This is to ensure identifying default is doable for this dataset. Otherwise, getting probability makes no sense
  
o Fit selected model to the analytics ready dataset. List outcomes from model fitting.
  I explored'LogisticRegression','DecisionTreeClassifier','RandomForestClassifier','AdaBoostClassifier',
  'GradientBoostingClassifier' for classfication. Due to the time limitation, I didnot try other methods, such as ANN, KNN. 
  Finally, I use logisticRegression to output probability of default on test data set. Because the F1-score for default is not   as high as nondefault, only around 0.52(GBoost).  So, I think, in real world application, we can manually adjust the boundary   of non default vs default to be P = less than 0.5, to increase recall 
  
o Evaluate model performance on held-out/testing dataset.
    On held-out for test. F1 score, accuracy are all reported.  
    If under sampling, F1 can be balanced to be 0.7 for both default and nondefault, accuracy also around 0.71
    If over sampling, F1 is high 0.87 for nondefault, 0.52 for default, accuracy is around 0.81
    
o What other options would you’ve considered (in solving the problem), if you had additional time?
    I only have a day this project, a lot more can be done to improve the model
    1. Could do more feature engineering. I didnot handle X5-X11 at all, which could be important 
    2. The parameters are not optimized yet. Gridsearch takes too long   
    3. I also could try ANN, KNN, Naive Bayes
    4. For the simplicity of geting probability, I only used logistic regression to estimate probablity of default
    
Thank you very much for the invitation!
Best
Ye Yuan