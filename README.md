# credit-default-demographics

Business Question:
What drives credit card defaults and how can we reduce them?

Summary
This project is focused on identifying patterns and predicting the number of credit defaults based on the specific conditions (default payments, demographic information, credit data, history of payment and bill statements). The poorly coded data in the dataset was altered prior to running our model. Using a logit classifier regression model better analyzed the relationship between our 1 dependent variable and the independent variables. With the accuracy percentage cutoff as our hyperparameter with a value of 0.51, anything below is a non-default and anything above is a default.  

Conclusion n/
We expected better results from the Logit regression due to its powerful capability to solve binary classification problems. Perhaps we could have done a better job tuning the prameters of the model or selecting different features. Despite the overall accuracy score, we were surprised by the precision and recall statistics.

                     Predicted Group 0  	  Predicted Group 1
Actual group 0              4484                	185
Actual group 1               1054                	264

                  Precision   	  Recall     F1-score
          0         0.810     	   0.960     	0.879
          1         0.588     	   0.200     	0.299
   Accuracy         0.793

While the model is useful for predicting non-defaults correctly, it falters in predicting defaults. Future work of this project could involve removing demographic variables that aren't viable for analysis. Additionally, comparing multiple models such as XG boost and random forest and using the model with the highest overall AUC would benefit the analysis. This model potentially has effective real world utility for banks. The real world implications could perhaps be employed by banks to reduce loan default losses and predict default behaviors of their customers.
