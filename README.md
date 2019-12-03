# Naive_Bayes_Classifier

This is a hands-on practice to understand about the Naive Bayes Classifier through a tutorial offered by [Analyticsvidhya](https://www.analyticsvidhya.com/blog/2017/09/naive-bayes-explained/?). It explains about the Naive Bayes Classifier and provides one simple problem and its solution in Python code.


### Understanding on the Naive Bayes

* According to [Wikipedia](https://en.wikipedia.org/wiki/Naive_Bayes_classifier), in machine learning, naïve Bayes classifiers are a family of simple "probabilistic classifiers" based on applying Bayes' theorem with strong (naïve) independence assumptions between the features. They are among the simplest Bayesian network models.
* A Naive Bayes classifier assumes that the presence of a particular feature in a class is unrelated to the presence of any other feature [(Analyticsvidhya)](https://www.analyticsvidhya.com/blog/2017/09/naive-bayes-explained/?).
* According to [scikit_learn.com](https://scikit-learn.org/stable/modules/naive_bayes.html), Naive Bayes methods are a set of supervised learning algorithms based on applying Bayes’ theorem with the “naive” assumption of conditional independence between every pair of features given the value of the class variable. ... In spite of their apparently over-simplified assumptions, naive Bayes classifiers have worked quite well in many real-world situations, famously document classification and spam filtering.

### Pros and Conc of Naive Bayes [Source](https://www.analyticsvidhya.com/blog/2017/09/naive-bayes-explained/?)
* Pros:
  1. It is easy and fast to predict class of test data set. It also perform well in multi class prediction
  2. When assumption of independence holds, a Naive Bayes classifier performs better compare to other models like logistic regression and you need less training data.
  3. It perform well in case of categorical input variables compared to numerical variable(s). For numerical variable, normal distribution is assumed (bell curve, which is a strong assumption).
