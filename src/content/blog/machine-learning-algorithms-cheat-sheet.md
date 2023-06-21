---
title: "Machine Learning Algorithms Cheat Sheet"
description: "...."
pubDate: "2021-02-09"
categories: 
  - "machine-learning"
---

[![Machine Learning Algorithms Cheat Sheet and how to choose an algorithm](/images/Machine%2BLearning%2BAlgorithms.png)](https://1.bp.blogspot.com/-dzztxX7TY98/YCIIdwQk9tI/AAAAAAAAPlc/uNB_A8ZNlTcb1khH1rKQcByJWiS945PjACLcBGAsYHQ/s1280/Machine%2BLearning%2BAlgorithms.png)

With the evolution of artificial intelligence, computer science researchers are constantly suggesting new approaches to make computers even more autonomous and capable of performing various tasks with precision. Traditionally, programmers have always developed systems by clearly specifying each step in code. For this, software engineers needed to know the problems they were trying to solve and have a good idea of ​​all the variables and possibilities involved. Machine Learning (ML) is a subfield of artificial intelligence that aims to solve more complex problems, of which programmers still do not have such a wide knowledge. [Learn what is machine learning from my previous article.](https://www.buddhilive.com/2020/06/25/what-is-machine-learning-a-brief-introduction/) 

## **Machine Learning Methods?**

Here, we will discuss the main methods of ML and their characteristics.

### 1\. Supervised learning

In Supervised Learning, we provide training data with their desired output (i.e. labels). So, we train the model using that data until it predicts the answers accurately. This is the most common method used. This is used for image recognition, object detection, face detection, voice recognition etc. Most common example for this is to teach a machine to recognize and categorize emails as spam or non-spam.

The results of this type of algorithms are usually marked as classification and regression. Classification algorithms finds a way of mapping equal elements in specific categories, as in the example above, "spam" and "non-spam". Regression models focus on identifying a trend for data that even allows predicting the future based on historical data. 

### 2\. Unsupervised learning

In unsupervised learning, we provide training data only. The machine learning algorithms try to find clusters of data based on their similar features. In supervised learning we use structured data, but in unsupervised learning we don't use structured data. It is up to the machine learning algorithm to find hidden structures in the data.

Unsupervised machine learning can be used in recommendation systems. It is widely used in e-commerce stores, to recommend products that may be interesting to the customer who visits the site. Similarly, there are streaming services that suggest music or videos to the user based on user preferences. **YouTube**, **Netflix** and **Amazon** use this approach to create their recommendation algorithms. 

### 3\. Reinforcement learning

In reinforcement learning, we let the computer to interact with a specific environment and perform actions. When the computer performs correct action, we reward it, if not we punish it. Well, the goal of the machine learning algorithm is to collect maximum rewards. This is like trial and error training.

Reinforcement learning was inspired by behavioral psychologists, who believed in the effectiveness of rewards and punishments in the education of human beings. It also recalls the procedure for training domestic animals.

It is, therefore, a method based on building experience. From this, the algorithm knows which paths are better than others and which processes are more agile.

This approach is commonly used in game development and autonomous vehicles. AI agents like AlphaGo which defeated world best Go players are trained using reinforcement learning. Such systems learn from multiple attempts, which involve mistakes like a bad move or a collision with an obstacle.

[![Popular machine learning algorithms](/images/machine-learning-algorithms.png)](https://1.bp.blogspot.com/-wBf3bnkqK7Q/YCIRew_N22I/AAAAAAAAPls/d4_KH2awEPgEFbyGXLUMGdimTs5HYiIAwCLcBGAsYHQ/s1366/machine-learning-algorithms.png)

##  What are Most Popular Machine Learning Algorithms?

There are lots of algorithms used in machine learning, each with a specific purpose. The algorithm you choose depends on the problem you want to solve. Here are the most popular machine learning algorithms and a brief introduction for each algorithm. We’ll discuss each algorithm in detail in separate articles.

1. **Linear Regression**

Linear regression is used to find the relationship between independent and dependent variables by fitting a best line. This line is known as the “Regression Line”. This is used to predict a value based on continues variables. For instance, if you have a price list of apartments based on the area and number of rooms, you can find the relationship of those variables to estimate the price of apartment for custom given area or number of rooms.

2. **Logistic Regression**

Logistic Regression is used for binary classification (e.g. true/false, yes/no, pass/fail etc.). It helps predict the probability of an event by fitting data to a logit function. This can be use for email spam filtering system which detects whether an email is spam or no-spam.

3. **Decision Tree**

Decision Tree is a supervised learning algorithm that is mostly used for classification problems. It can be used for both categorical and continuous dependent variables. Decision Tree algorithm works by splitting the population into two or more homogeneous sets based on most significant attributes (independent variables).

4. **SVM (Support Vector Machine)**

Support Vector Machine is a classification algorithm in which raw data is plotted as points in an n-dimensional space (**_n_**is the number of features) using the value of each feature as the value of coordinate.

5. **Naïve Bayes**

Naïve Bayes is also a classification technique that assumes the presence of a particular feature in a class is unrelated to the presence of any other feature even if these features are related to each other. For example, a fruit will be assumed as an orange if it is round, orange in color and 6cm in diameter. Although these features depend on each other when identifying the orange, naïve Bayes classifier would consider all of these features contribute independently to the probability that this fruit is an orange.

6. **kNN (k- Nearest Neighbors)**

kNN stores all available cases and classifies any new cases by taking a majority vote of its k neighbors. It’s something like this; if you want to know details about a certain person, you can get details by talking to that persons’ friends or family. kNN algorithm works in the same way. Although this algorithm can be used in both classification and regression problems, it's widely used to solve classification problems.

7. **K-Means**

K-Means is an unsupervised algorithm that solves clustering problems by classifying datasets into a particular number of clusters (which is known as K). All the data points within a cluster are homogenous and heterogeneous from the data in other clusters.

8. **Random Forest**

Random Forest is a collective of decision trees. In this algorithm each tree classifies an object based on its attributes and the tree votes for that class. The forest chooses the classification having the most votes.

9. **Dimensionality Reduction Algorithms**

As many companies collect and store large amounts of data these days, we can find large amounts of data with many features. This sounds good, but when it comes to choose the best features to use for building a machine learning model. So, basically, Dimensionality Reduction Algorithms helps to identifying significant patterns and variables out of these large number of datasets.

10. **Gradient Boosting Algorithms**

Gradient Boosting Algorithms are used to handled massive loads of data to make predictions with high accuracy. There are several Gradient Boosting Algorithms in use. Following are the most common algorithms in use;

1. GBM
2. XGBoost
3. LightGBM
4. CatBoost 

[![Machine Learning algorithms and their applications](/images/machine-learning-algorithms-usecases.png)](https://1.bp.blogspot.com/-xn0wwlQ-WXU/YCIRwJSbr-I/AAAAAAAAPl0/LAq7gQMCNb8aSowliP7DWRfTd5ON4NIOQCLcBGAsYHQ/s1366/machine-learning-algorithms-usecases.png)

## How to choose the ideal algorithm?

As there are several ways to reach a result with ML, and because there are several approaches, it is necessary to know how to choose the most appropriate algorithm for the proposed problem. We'll look at some tips below. 

### **1\. Purpose of the problem**

It is important to know well the purpose and context of the case that must be processed by the machine, with specific details, as they help to select the best way to handle the data.

For example, if there is a well-defined goal, with known outputs, the ideal algorithm could be a supervised learning method. 

### **2\. Amount of data**

Another relevant aspect is the amount of data that will be used to feed the ML model. Neural networks, for example, usually need large sets of input. In addition, if the dataset is very large and the algorithm is too complex, it may be necessary to make an assessment regarding the computational capacity necessary for the execution of the algorithm. 

### **3\. Problem complexity and accuracy**

The complexity of the problem is also an important aspect, as this determines the degree of accuracy desired. Thus, it is possible to select which algorithm best fits this degree of accuracy by analyzing factors such as what are the consequences that can bring if the model output an incorrect prediction.

### **4\. Time**

Finally, time must be considered when choosing the type of Machine Learning algorithm that best solves the case. Because some problems require real-time decisions.

#### Summary

In this article, we learn how Machine Learning algorithms differ and are classified into three major categories and smaller subcategories. Each has its own characteristic and strengths. It is hard to say this algorithm is better than that algorithm, because it depends on the problem you are going to solve. Here we discuss the machine learning algorithm in brief to keep the article short. We’ll learn these algorithms with code examples in the future articles.
