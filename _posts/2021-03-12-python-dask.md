---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Powered by Dask"
tags: ['Python', 'parallel computing']
image: "2021-03-12/py-lib.png"
identifier: 3
---
Dask is a flexible library for parallel computing in Python. Dask uses existing Python APIs and data structures to make it easy to switch between NumPy, pandas, scikit-learn to their Dask-powered equivalents. 

Author and collect by: Cell, Sheryl

<!--more-->

<blockquote class="tip">
  <strong>Dask</strong> is open source and freely available. It is developed in coordination with other community projects like NumPy, pandas, and scikit-learns. Dask's schedulers scale to thousand-node clusters and its algorithms have been tested on some of the largest supercomputers in the world. Dask exposes lower-level APIs letting you build custom systems for in-house applications. This helps open source leaders parallelize their own packages and helps business leaders scale custom business logic.

</blockquote>

<div class="list-of-contents">
  <h4>Contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization">Dask</h4>
Dask is composed of two parts.

<hr class="with-margin">
<h4 class="header" id="quantization">1: Dynamic task scheduling</h4>

<br>
Dynamic task scheduling optimized for computation. This is similar to Airflow, Luigi, Celery, or Make, but optimized for interactive computational workloads.
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">2: “Big Data” </h4>

“Big Data” collections like parallel arrays, dataframes, and lists that extend common interfaces like NumPy, Pandas, or Python iterators to larger-than-memory or distributed environments. These parallel collections run on top of dynamic task schedulers.
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Emphasizes</h4>

Dask emphasizes the following virtues:<br>

<strong>Familiar:</strong> Provides parallelized NumPy array and Pandas DataFrame objects<br>

<strong>Flexible:</strong> Provides a task scheduling interface for more custom workloads and integration with other projects.<br>

<strong>Native:</strong> Enables distributed computing in pure Python with access to the PyData stack.<br>

<strong>Fast:</strong> Operates with low overhead, low latency, and minimal serialization necessary for fast numerical algorithms<br>

<strong>Scales up:</strong> Runs resiliently on clusters with 1000s of cores<br>

<strong>Scales down:</strong> Trivial to set up and run on a laptop in a single process<br>

<strong>Responsive:</strong> Designed with interactive computing in mind, it provides rapid feedback and diagnostics to aid humans.<br>

![daskoverviewr]({{ site.baseurl }}/assets/img/2021-03-12/dask-overview.png){: .center-image}
<em class="figure">Fig 1. Dask Overview</em>
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">user interface</h4>

Dask DataFrame mimics Pandas
<br>

Dask dataframes scale pandas workflows, enabling applications in time series, business intelligence, and general data munging on big data.
<br>

![pd]({{ site.baseurl }}/assets/img/2021-03-12/pd.png){: .center-image}
<em class="figure">Fig 2. Dask DataFrame mimics Pandaso</em>
<br>


Dask Array mimics NumPy
<br>

Dask arrays scale NumPy workflows, enabling multi-dimensional data analysis in earth science, satellite imagery, genomics, biomedical applications, and machine learning algorithms.
<br>

![np]({{ site.baseurl }}/assets/img/2021-03-12/np.png){: .center-image}
<em class="figure">Fig 3. Dask Array mimics NumPy</em>
<br>

Dask Bag mimics iterators, Toolz, and PySpark
<br>

![pyspark]({{ site.baseurl }}/assets/img/2021-03-12/pyspark.png){: .center-image}
<em class="figure">Fig 4. Dask Bag mimics iterators, Toolz, and PySpark</em>
<br>

scikit-learn: Dask-ML scales machine learning APIs like scikit-learn and XGBoost to enable scalable training and prediction on large models and large datasets.
<br>

![mllib]({{ site.baseurl }}/assets/img/2021-03-12/xgboost.png){: .center-image}
<em class="figure">Fig 5. Dask-ML XGBoost</em>
<br>


![modelsize]({{ site.baseurl }}/assets/img/2021-03-12/modelsize.png){: .center-image}
<em class="figure">Fig 6. Scaling Model Size</em>
<br>

<hr class="with-margin">
### References

<ol>
  <li><a href="https://dask.org/">Dask natively scales Python</a></li>
</ol>

<ol>
  <li><a href="https://github.com/dask/dask-ml/labels/Roadmap">Dask-ML Roadmap</a></li>
</ol>

<hr class="with-margin">

![schedule]({{ site.baseurl }}/assets/img/2021-03-12/grid_search_schedule.gif){: .autofit-image}
<br>