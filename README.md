Problem Statement
----
Develop a classification model that can distinguish which of two subreddits, ([r/menstruation](https://www.reddit.com/r/menstruation) or [r/BabyBumps](https://www.reddit.com/r/BabyBumps)), a particular post belongs to.


## Executive Summary
We cleaned and analyzed 2 features (post text and post title) which we engineered by way of Count Vectorizing. We removed English stop words, stripped ASCII accents for both features.  This resulted in a 393 features which we fed into 2 variations of Logistic Regression, Decision Tree, Random Forest and Multinomial NB models each.

My second Multinomial Naive Bayes model performed the best. With the best parameters being?-?alpha: 0 and fit_prior: False. The accuracy score on the training data was 92.4% and on unseen data it came out to be 92.2%. This means our model is slightly and probably inconsequentially overfit. This also means that 92.2% of our posts will be accurately classified by our model.

#### Recommendations

* Go with Multinomial Naive Bayes Model
  * Version 2 handled bias/variance the best

* Spend more time with current features
  * e.g. Engineer a character or word length feature

* Explore new features
  * Upvotes
  * Post comments

   
#### Our presentation can be found [here.](https://docs.google.com/presentation/d/1S3R8KSKmX8M_uOtiXYiAQbVpRUHqMC8QfxfBW7Zx18k/edit?usp=sharing) I also have [an article featured on Towards Data Science](https://towardsdatascience.com/classifying-reddit-posts-with-natural-language-processing-and-machine-learning-695f9a576ecb) that walks you through my data science process.
