---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "A Tour of Machine Learning Ten Algorithms"
tags: ['Machine Learning', 'Alogrithms']
image: "2019-11-15/machine-learning-algorithms-cover.png"
identifier: 3
---

Machine learning algorithms are programs that can learn from data and improve from experience, without human intervention. 
Learning tasks may include learning the function that maps the input to the output, learning the hidden structure in unlabeled data; 
or ‘instance-based learning’, where a class label is produced for a new instance by comparing the new instance (row) to instances from 
the training data, which were stored in memory. ‘Instance-based learning’ does not create an abstraction from specific instances.
<br>
Machine learning is also often referred to as predictive analytics, or predictive modelling.
<br>

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
<em class="figure">Fig 1. supervised-machine-learning</em>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/ml_2.png){: .center-image}
<em class="figure">Fig 2. supervised vs. unsupervised</em>


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
<em class="figure">Fig 3. Supervised-and-unsupervised-machine-learning</em>

<hr class="with-margin">
<h4 class="header" id="quantization">Semi-supervised learning</h4>
Semi-supervised learning is similar to supervised learning, but instead uses both labelled and unlabelled data. Input data is a mixture of labeled and unlabelled examples. Labelled data is essentially information that has meaningful tags so that the algorithm can understand the data, whilst unlabelled data lacks that information. By using this
combination, machine learning algorithms can learn to label unlabelled data.


![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/semi-supervised_1.png){: .center-image}
<em class="figure">Fig 4. Semi-Supervised machine learning</em>

<hr class="with-margin">
<h4 class="header" id="casestudy">Reinforcement learning</h4>
Reinforcement Learning is an aspect of Machine learning where an agent learns to behave in an environment, 
by performing certain actions and observing the rewards/results which it get from those actions

Reinforcement learning focuses on regimented learning processes, where a machine learning algorithm is provided with a set of actions,
 parameters and end values. By defining the rules, the machine learning algorithm then tries to explore different options and possibilities,
 monitoring and evaluating each result to determine which one is optimal. Reinforcement learning teaches the machine trial and error. 
 <br>
 It learns from past experiences and begins to adapt its approach in response to the situation to achieve the best possible result.

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/reinforcementlearning_1.png){: .center-image}
<em class="figure">Fig 5. Reinforcement learning</em>


<hr class="with-margin">
<h4 class="header" id="casestudy">Common and popular machine learning algorithms</h4>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/MachineLearningAlgorithms_0.png){: .center-image}
<em class="figure">Fig 5. MachineLearning Algorithms</em>
<br>
**Regression Algorithms**
<br>
**Decision Tree Algorithms**
<br>
**Naïve Bayes Classifier Algorithm**
<br>
**Clustering Algorithms: (Unsupervised Learning)**
<br>
**Support Vector Machines**
<br>
**Principal Component Analysis**
<br>
**Artificial Neural Networks Algorithms(Reinforcement Learning)**
<br>
**Deep Learning Algorithms**
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/machine-learning-cheet-sheet.png){: .center-image}
<em class="figure">Fig 5.[machine-learning-cheet-sheet](https://blogs.sas.com/content/subconsciousmusings/2017/04/12/machine-learning-algorithm-use/)</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/ml_map.png){: .center-image}
<em class="figure">Fig 5. Usage examples</em>
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-15/Types-of-Machine-Learning-algorithms.png){: .center-image}
<em class="figure">Fig 5. Usage examples</em>




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
