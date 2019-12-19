---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Installing Anaconda in Hadoop - Using Anaconda with Spark"
tags: ['python', 'Anaconda', 'Hadoop']
image: "2019-11-11/installConda_14.PNG"
identifier: 3
---
Anaconda is a free and open-source distribution of the Python and R programming languages 
for scientific computing, that aims to simplify package management and deployment. 
Package versions are managed by the package management system conda.
Author and collect by: Sheryl

<!--more-->

<blockquote class="tip">
The open-source <strong>Anaconda</strong> Distribution is the easiest way to perform Python/R data science
 and machine learning on Linux, Windows, and Mac OS X. With over 15 million users worldwide, it is the industry 
 standard for developing, testing, and training on a single machine, enabling individual data scientists to:
   <ol>    
    <li>
      Quickly download 1,500+ Python/R data science packages.
    </li>
    <li>
      Manage libraries, dependencies, and environments with <a href="https://conda.io/en/latest/">Conda</a>.
    </li>
    <li>
      Develop and train machine learning and deep learning models with scikit-learn, TensorFlow, and Theano
    </li>
    <li>
	Analyze data with scalability and performance with Dask, NumPy, pandas, and Numba
	</li>
    <li>
	Visualize results with Matplotlib, Bokeh, Datashader, and Holoviews
	</li>
  </ol>
</blockquote>

<div class="list-of-contents">
  <h4>Post contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization">Anaconda Installation in Hadoop</h4>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_1.PNG){: .center-image}
<em class="figure">Fig 1. Upload anaconda install file to Hadoop file system.
</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_2.PNG){: .center-image}
<em class="figure">Fig 2. Login as root. find Anaconda install file, and bash to install</em>
<br>


![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_3.PNG){: .center-image}
<em class="figure">Fig 3. Default settings.</em>
<br>


![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_4.PNG){: .center-image}
<em class="figure">Fig 4. </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_5.PNG){: .center-image}
<em class="figure">Fig 5. </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_6.PNG){: .center-image}
<em class="figure">Fig 6. </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_7.PNG){: .center-image}
<em class="figure">Fig 7. </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_8.PNG){: .center-image}
<em class="figure">Fig 8.update packages.</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_9.PNG){: .center-image}
<em class="figure">Fig 9. </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_10.PNG){: .center-image}
<em class="figure">Fig 10. </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_11.PNG){: .center-image}
<em class="figure">Fig 11. using ipython, or jupyter </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_12.PNG){: .center-image}
<em class="figure">Fig 12. install keras deep learning packages</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_13.PNG){: .center-image}
<em class="figure">Fig 13. Here is anaconda installer archive. Install another version, Anaconda2</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2019-11-11/installConda_14.PNG){: .center-image}
<em class="figure">Fig 14. After install Anaconda2, and testing by suing pyspark. 
For HDP 3.1, still using python2, so you could install Anaconda2 and Anaconda3, and specific coda version/direction to use.</em>
<br>


<hr class="with-margin">
### References

<ol>
  <li><a href="https://docs.anaconda.com/anaconda-scale/spark/">Using Anaconda with Spark</a></li>
  <li><a href="https://enterprise-docs.anaconda.com/en/latest/data-science-workflows/templates/spark-hadoop.html">Hadoop Spark</a></li>
  <li><a href="https://dzone.com/articles/making-python-on-apache-hadoop-easier-with-anacond">Making Python on Apache Hadoop Easier with Anaconda and CDH</a></li>
</ol>
