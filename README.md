# Naive_Bayes_Classifier

This is a hands-on practice to understand the Naive Bayes Classifier through a tutorial offered by [Analyticsvidhya](https://www.analyticsvidhya.com/blog/2017/09/naive-bayes-explained/?). It explains about the Naive Bayes Classifier and provides one problem and its solution in Python code. The problem is one of the most famous problem: Titanic, predicting survival on the Titanic.

### Bayes Theorem
![Equation](https://www.analyticsvidhya.com/wp-content/uploads/2015/09/Bayes_rule-300x172.png)
      
### Understanding on the Naive Bayes

* According to [Wikipedia](https://en.wikipedia.org/wiki/Naive_Bayes_classifier), in machine learning, naïve Bayes classifiers are a family of simple "probabilistic classifiers" based on applying Bayes' theorem with strong (naïve) independence assumptions between the features. They are among the simplest Bayesian network models.
* A Naive Bayes classifier assumes that the presence of a particular feature in a class is unrelated to the presence of any other feature [(Analyticsvidhya)](https://www.analyticsvidhya.com/blog/2017/09/naive-bayes-explained/?).
* According to [scikit_learn.com](https://scikit-learn.org/stable/modules/naive_bayes.html), Naive Bayes methods are a set of supervised learning algorithms based on applying Bayes’ theorem with the “naive” assumption of conditional independence between every pair of features given the value of the class variable. ... In spite of their apparently over-simplified assumptions, naive Bayes classifiers have worked quite well in many real-world situations, famously document classification and spam filtering.

### Pros and Conc of Naive Bayes [(Source)](https://www.analyticsvidhya.com/blog/2017/09/naive-bayes-explained/?)
* Pros:
  1. It is easy and fast to predict class of test data set. It also perform well in multi class prediction
  2. When assumption of independence holds, a Naive Bayes classifier performs better compare to other models like logistic regression and you need less training data.
  3. It perform well in case of categorical input variables compared to numerical variable(s). For numerical variable, normal distribution is assumed (bell curve, which is a strong assumption).
* Cons:
  1. If categorical variable has a category (in test data set), which was not observed in training data set, then model will assign a 0 (zero) probability and will be unable to make a prediction. This is often known as “Zero Frequency”. To solve this, we can use the smoothing technique. One of the simplest smoothing techniques is called Laplace estimation.
  2. On the other side naive Bayes is also known as a bad estimator, so the probability outputs from predict_proba are not to be taken too seriously.
  3. Another limitation of Naive Bayes is the assumption of independent predictors. In real life, it is almost impossible that we get a set of predictors which are completely independent.
  
### Applications of Naive Bayes Algorithms
* **Real time Prediction**: Naive Bayes is an eager learning classifier and it is sure fast. Thus, it could be used for making predictions in real time.
* **Multi class Prediction**: This algorithm is also well known for multi class prediction feature. Here we can predict the probability of multiple classes of target variable.
* **Text classification/ Spam Filtering/ Sentiment Analysis**: Naive Bayes classifiers mostly used in text classification (due to better result in multi class problems and independence rule) have higher success rate as compared to other algorithms. As a result, it is widely used in Spam filtering (identify spam e-mail) and Sentiment Analysis (in social media analysis, to identify positive and negative customer sentiments)
* **Recommendation System**: Naive Bayes Classifier and Collaborative Filtering together builds a Recommendation System that uses machine learning and data mining techniques to filter unseen information and predict whether a user would like a given resource or not

### Example Problem statement:
#### Players will play if weather is sunny. Is this statement correct?


### Solution:
1. Step1: Convert a data set given in a table form with two columns, weather and play, into a frequency table

2. Step2: Create Likelihood table by finding the probabilities, for example, a probability(overcase and playing) = 0.64
![Equation](https://www.analyticsvidhya.com/wp-content/uploads/2015/08/Bayes_41.png)

3. Step3: Use the Naive Bayesian equation to calculate the posterior probability for each class. The class with the highest posterior probability is the outcome of prediction.
  - Example: <br/>
      P(Yes|Sunny) = P(Sunny|Yes) * P(Yes) / P(Sunny)<br/>
      Since P(Sunny|Yes) = 3/9 = 0.33, P(Sunny) = 5/14 = 0.36, and P(Yes) = 0.64,
      P(Yes|Sunny) = 0.33 * 0.64 / 0.36 = 0.60
