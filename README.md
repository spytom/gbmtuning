# gbmtuning: Tuning Gradient Boosting (GBM) in Python 
Author: Thomas Spycher, March 3rd, 2018


GBM is a highly popular prediction model among data scientists or as top Kaggler Owen Zhang describes it: "My confession: I (over)use GBM. When in doubt, use GBM."

[GradientBoostingClassifier](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html) from sklearn is a popular and user friendly application of Gradient Boosting in Python (another nice and even faster tool is xgboost). Apart from setting up the feature space and fitting the model, parameter tuning is a crucial task in finding the model with the highest predictive power. 

* This code provides an example of GBM parameter tuning of a classification model in Pyton
* It applies parameter tuning to the HP Lab Spam dataset; we focus on improving accuracy of the model and abstract from preferences regarding false negative or false positive predictions (For a spam filter, the cost of false positive predictions (regular emails reported as spam) are likely much higher than from false negative (spam emails not reported as spam)* For a formal discussion of Gradient Boosting see for example [these lecture notes](http://cs229.stanford.edu/extra-notes/boosting.pdf). 
* The tuning process is based on recommendations by [Owen Zhang](https://nycdatascience.com/blog/meetup/featured-talk-1-kaggle-data-scientist-owen-zhang/) as well as suggestions on [Analytics Vidhya](https://www.analyticsvidhya.com/blog/2016/02/complete-guide-parameter-tuning-gradient-boosting-gbm-python/).
