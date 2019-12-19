---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "A Tour of Machine Learning Ten Algorithms"
tags: ['Machine Learning', 'Alogrithms']
image: "2019-11-15/machine-learning-algorithms-cover.png"
identifier: 3
---

Machine learning algorithms are programs that can learn from data and improve from experience without human intervention. 
Learning tasks may include learning the function that maps the input to the output, learning the hidden structure in unlabeled data; 
or 'instance-based learning', where a class label is produced for a new instance by comparing the new instance (row) to instances from 
the training data, which were stored in memory. ‘Instance-based learning’ does not create an abstraction from specific instances.
<br>
Machine learning is also often referred to as predictive analytics, or predictive modelling.
<!--more-->

<blockquote class="tip">
<strong> Machine learning</strong> uses programmed algorithms that receive and analyse input data to predict output values within an acceptable range. 
 As new data is fed to these algorithms, they learn and optimise their operations to improve performance, developing ‘intelligence’ over time.
There are four types of machine learning algorithms: <strong> supervised, semi-supervised, unsupervised and reinforcement</strong>.
</blockquote>

<div class="list-of-contents">
  <h4>Post contents</h4>
  <ul></ul>
</div>

<hr class="with-margin">
<h4 class="header" id="intro">Supervised learning</h4>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/ml_glance_1.jpg){: .center-image}
<em class="figure">Fig 1. machine-learning at a glance</em>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/ml_glance_2.png){: .center-image}
<em class="figure">Fig 2. machine-learning</em>

In **supervised learning**, the machine is taught by example (traning data). There are known-labeled data .
The operator provides the machine learning algorithm with a known dataset that includes desired inputs and outputs, 
and the algorithm must find a method to determine how to arrive at those inputs and outputs. 
While the operator knows the correct answers to the problem, the algorithm identifies patterns in data, 
learns from observations and makes predictions. The algorithm makes predictions and 
is corrected by the operator – and this process continues until the algorithm achieves a high level of accuracy/performance.

<blockquote class="algo">
  <ol>    
    <li>
      Classification: In classification tasks, the machine learning program must draw a conclusion from observed values and determine to what category new observations belong. For example, when filtering emails as ‘spam’ or ‘not spam’, the program must look at existing observational data and filter the emails accordingly.
    </li>
    <li>
      Regression: In regression tasks, the machine learning program must estimate – and understand – the relationships among variables. Regression analysis focuses on one dependent variable and a series of other changing variables – making it particularly useful for prediction and forecasting..
    </li>
    <li>
      Forecasting: Forecasting is the process of making predictions about the future based on the past and present data, and is commonly used to analyse trends.
    </li>
  </ol>
</blockquote>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/supervised-machine-learning.png){: .center-image}
<em class="figure">Fig 3. supervised-machine-learning</em>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/ml_2.png){: .center-image}
<em class="figure">Fig 4. supervised vs. unsupervised</em>


<hr class="with-margin">
<h4 class="header" id="implementation">Unsupervised learning</h4>

The machine learning algorithm studies data to identify patterns. Input data is not labeled and does not have a known result. There is no answer key or human operator to provide instruction. 
Instead, the machine determines the correlations and relationships by analysing available data. 
In an unsupervised learning process, the machine learning algorithm is left to interpret large data sets and address that data accordingly. 
The algorithm tries to organise that data in some way to describe its structure. 
This might mean grouping the data into clusters or arranging it in a way that looks more organised.
<br>
As it assesses more data, its ability to make decisions on that data gradually improves and becomes more refined.
<blockquote class="algo">
  <ol>    
    <li>
    Clustering: Clustering involves grouping sets of similar data (based on defined criteria). It’s useful for segmenting data into several groups and performing analysis on each data set to find patterns.
	</li>
    <li>
	Dimension reduction: Dimension reduction reduces the number of variables being considered to find the exact information required.
	</li>
  </ol>
</blockquote>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/Supervised-and-unsupervised-machine-learning.png){: .center-image}
<em class="figure">Fig 5. Supervised-and-unsupervised-machine-learning</em>

<hr class="with-margin">
<h4 class="header" id="quantization">Semi-supervised learning</h4>
Semi-supervised learning is similar to supervised learning, but instead uses both labelled and unlabelled data. Input data is a mixture of labeled and unlabelled examples. Labelled data is essentially information that has meaningful tags so that the algorithm can understand the data, whilst unlabelled data lacks that information. By using this
combination, machine learning algorithms can learn to label unlabelled data.


![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/semi-supervised_1.png){: .center-image}
<em class="figure">Fig 6. Semi-Supervised machine learning</em>

<hr class="with-margin">
<h4 class="header" id="casestudy">Reinforcement learning</h4>
Reinforcement Learning is an aspect of Machine learning where an agent learns to behave in an environment, 
by performing certain actions and observing the rewards/results which it get from those actions

Reinforcement learning focuses on regimented learning processes, where a machine learning algorithm is provided with a set of actions,
 parameters and end values. By defining the rules, the machine learning algorithm then tries to explore different options and possibilities,
 monitoring and evaluating each result to determine which one is optimal. Reinforcement learning teaches the machine trial and error. 
 <br>
 It learns from past experiences and begins to adapt its approach in response to the situation to achieve the best possible result.

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/reinforcementlearning_1.png){: .small70-image}
<em class="figure">Fig 7. Reinforcement learning</em>


<hr class="with-margin">
<h4 class="header" id="casestudy">Common and popular machine learning algorithms</h4>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/MachineLearningAlgorithms_0.png){: .small70-image}
<em class="figure">Fig 8. MachineLearning Algorithms</em>
<br>
**Regression Algorithms**
<br>
Regression algorithms predict the output values based on input features from the data fed in the system. 
The go-to methodology is the algorithm builds a model on the features of training data and using the model to predict value for new data.
<blockquote class="algo">
  <ol>    
    <li>
    Linear regression is the most basic type of regression. Simple linear regression allows us to understand the relationships between two continuous variables.
	</li>
    <li>
	Logistic regression focuses on estimating the probability of an event occurring based on the previous data provided. 
	It is used to cover a binary dependent variable, that is where only two values, 0 and 1, represent outcomes.
	</li>
  </ol>
</blockquote>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/regression_1.png){: .small70-image}
<em class="figure">Fig 10. Regression</em>regression_2.png
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/regression_2.png){: .small70-image}
<em class="figure">Fig 11. Regression</em>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/regression_3.png){: .small70-image}
<em class="figure">Fig 12. Regression</em>

<br>
**Decision Tree Algorithms**
<br>
A decision tree is a flow-chart-like tree structure that uses a branching method to illustrate every possible outcome of a decision. 
Each node within the tree represents a test on a specific variable – and each branch is the outcome of that test.
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/what-is-a-decision-tree.png){: .small70-image}
<em class="figure">Fig 13. Decision tree</em>

**Naïve Bayes Classifier Algorithm**
<br>
Bayesian methods are based on Bayes’ theorem and classifies every value as independent of any other value. 
It allows us to predict a class/category, based on a given set of features, using probability.
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/naive_bayes_icon.png){: .small70-image}
<em class="figure">Fig 14. Bayes</em>

More read about [Bayes theorem](https://luminousmen.com/post/data-science-bayes-theorem).
<br>
**Clustering Algorithms: (Unsupervised Learning)**
<br>
Clustering methods are typically organized by the modeling approaches such as centroid-based and hierarchal. 
All methods are concerned with using the inherent structures in the data to best organize the data into groups of maximum commonality.
<blockquote class="algo">
  <ol>    
    <li>
    The K Means Clustering algorithm is a type of unsupervised learning, which is used to categorise unlabelled data, i.e. data without defined categories or groups. The algorithm works by finding groups within the data, with the number of groups represented by the variable K. 
	It then works iteratively to assign each data point to one of K groups based on the features provided.
	</li>
    <li>
	Others
	</li>
  </ol>
</blockquote>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/k-means_1.png){: .small70-image}
<em class="figure">Fig 15. k-means</em>


<br>
**Support Vector Machines**
<br>
are supervised learning models that analyse data used for classification and regression analysis. They essentially filter data into categories, which is achieved by providing a set of training examples, each set marked as belonging to one or the other of the two categories. 
SVM The algorithm then works to build a model that assigns new values to one category or the other.

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/support-vector-machine-algorithm5.png){: .small70-image}
<em class="figure">Fig 16. SVM</em>


![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/SVM-process-example-on-two-dimensional-data.png){: .small70-image}
<em class="figure">Fig 17. SVM</em>
<br>
**Principal Component Analysis**
<br>
Principal component analysis (PCA) is a mathematical procedure that transforms a number of (possibly) correlated variables into a (smaller) number of uncorrelated variables called principal components.
Principal components analysis is similar to another multivariate procedure called Factor Analysis.
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/Principal+Component+Analysis.jpg){: .small70-image}
<em class="figure">Fig 18. PCA</em>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/pca_2.png){: .small70-image}
<em class="figure">Fig 19. PCA</em>

**Artificial Neural Networks Algorithms(Reinforcement Learning)**
<br>
ANN comprises ‘units’ arranged in a series of layers, each of which connects to layers on either side. ANNs are inspired by biological systems, such as the brain, and how they process information. ANNs are essentially a large number of interconnected processing elements, working in unison to solve specific problems.

ANNs also learn by example and through experience, and they are extremely useful for modelling non-linear relationships in high-dimensional data or where the relationship amongst the input variables is difficult to understand.
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/ann-1.png){: .small70-image}
<em class="figure">Fig 20.ANN</em>


**Deep Learning Algorithms**
<br>
Deep learning (also known as deep structured learning or hierarchical learning) is part of a broader family of machine learning methods based on artificial neural networks.
<br>
Deep learning algorithms run data through several “layers” of neural network algorithms, each of which passes a simplified representation of the data to the next layer.

Most machine learning algorithms work well on datasets that have up to a few hundred features, or columns. However, an unstructured dataset, like one from an image, has such a large number of features that this process becomes cumbersome or completely unfeasible. 
A single 800-by-1000-pixel image in RGB color has 2.4 million features – far too many for traditional machine learning algorithms to handle.
<br>
Many methods are concerned with very large datasets of labelled analog data, such as image, text. audio, and video.
<br>
Deep learning algorithms learn progressively more about the image as it goes through each neural network layer. 
Early layers learn how to detect low-level features like edges, and subsequent layers combine features from earlier layers into a more holistic representation. 
<br>
For example, a middle layer might identify edges to detect parts of an object in the photo such as a leg or a branch, while a deep layer will detect the full object such as a dog or a tree.


<blockquote class="algo">
  <ol>    
    <li>
    Convolutional Neural Network (CNN)
	</li>
    <li>
	Recurrent Neural Networks (RNNs)
	</li>
	<li>
	Long Short-Term Memory Networks (LSTMs)
	</li>
	<li>
	Others
	</li>
  </ol>
</blockquote>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/deeplearning_1.png){: .small70-image}
<em class="figure">Fig 21.deep learning</em>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/deeplearning_3.png){: .small70-image}
<em class="figure">Fig 22.deep learning</em>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/deeplearning_4.png){: .small70-image}
<em class="figure">Fig 23.deep learning</em>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/deeplearning_2.png){: .small70-image}
<em class="figure">Fig 24.deep learning</em>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/deeplearning_5.png){: .small70-image}
<em class="figure">Fig 25.deep learning</em>

<hr class="with-margin">
<h4 class="header" id="quantization">Machine learning algorithm selection</h4>
<br>
Know the questions before you begin to do a data analysis and one/many algorithms selection.
<blockquote class="algo">
  <ol>    
    <li>
    The size, quality, and nature of data.
	</li>
    <li>
	The available computational time
	</li>
	<li>
	Define the problem. What you want to do with the data, what answer you want to generate.
	</li>
	<li>
	The selected machine model in a pipline. whether you need to use final model to play a role in big data system, like hadoop, spark data stream.
	</li>
  </ol>
</blockquote>


![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/MathWorks_1500.jpg){: .small70-image}
<em class="figure">Fig 26. design engineering workflow</em>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/workflow_2.png){: .small70-image}
<em class="figure">Fig 27. Glance</em>


![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/machine-learning-cheet-sheet.png){: .small70-image}
<em class="figure">Fig 28.[machine-learning-cheet-sheet](https://blogs.sas.com/content/subconsciousmusings/2017/04/12/machine-learning-algorithm-use/)</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/ml_map.png){: .small70-image}
<em class="figure">Fig 29. Usage examples</em>
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/Types-of-Machine-Learning-algorithms.png){: .small70-image}
<em class="figure">Fig 30. Usage examples</em>

<hr class="with-margin">
### References
<ol>
  <li><a href="https://machinelearningmastery.com/a-tour-of-machine-learning-algorithms/">A Tour of Machine Learning Algorithms</a></li>
  <li><a href="https://www.kdnuggets.com/2016/08/10-algorithms-machine-learning-engineers.html">The 10 Algorithms Machine Learning Engineers Need to Know </a></li>
  <li><a href="https://www.dataquest.io/blog/top-10-machine-learning-algorithms-for-beginners/">The 10 Best Machine Learning Algorithms for Data Science Beginners</a></li>
  <li><a href="https://towardsdatascience.com/top-10-machine-learning-algorithms-for-data-science-cdb0400a25f9">Top 10 Machine Learning Algorithms for Data Sciencen</a></li>
  <li><a href="https://www.sas.com/en_ie/insights/articles/analytics/machine-learning-algorithms.html">A guide to machine learning algorithms and their applications</a></li>
  <li><a href="https://blogs.sas.com/content/subconsciousmusings/2017/04/12/machine-learning-algorithm-use/">Which machine learning algorithm should I use?</a></li>
</ol>
