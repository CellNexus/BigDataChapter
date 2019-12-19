---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Anaconda Installation in OS, and Hadoop"
tags: ['python', 'Anaconda', 'Installation']
image: "2019-11-01/anaconda_cover1.png"
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
<h4 class="header" id="intro">Anaconda Documentation for installation</h4>


[Download Anaconda Distribution](https://www.anaconda.com/distribution/).
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/anaconda_distribution_1.png){: .center-image}
<em class="figure">Fig 1. Anaconda Distribution</em>

<br>
[Installing Anaconda Distribution](https://docs.anaconda.com/anaconda/install/).
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/anaconda_install_1.png){: .center-image}
<em class="figure">Fig 2. Anaconda Document for installation</em>

<hr class="with-margin">
<h4 class="header" id="quantization">Install Anaconda on Ubuntu by using Oracle VirtualBox in Windows OS</h4>
To support all packages provided by Anaconda, here introduce install Anaconda in Ubuntu which is on VirtualBox.
If your computer is using Linux, MacOS or would like to use Anaconda in Windows, ignore this part.
<blockquote class="algo">
  <ol> 
    <li>
      Install Oracle VirtualBox on Windows OS.
    </li>  
    <li>
      Install Ubuntu on Oracle VirtualBox.
    </li>
    <li>
      Install Anaconda on Ubuntu.
    </li>
  </ol>
</blockquote>

<br>

For Install Oracle VirtualBox on Windows OS, please check the [HDF post](https://www.forparkinson.com/BigDataChapter/blog/2019/05/17/hortonworks-sandbox)

For install Ubuntu on VirtualBox:
<br>
Go to [Download Ubuntu Desktop](https://ubuntu.com/download/desktop).
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_0.png){: .center-image}
<em class="figure">Fig 0. Ubuntu download</em>

<br>
Open VM.
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_1.png){: .center-image}
<em class="figure">Fig 1. Start VM</em>
(In this Figure, there already has HDF and Ubuntu, will install another Ubuntu for this post)

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_2.png){: .center-image}
<em class="figure">Fig 2. Select New, and type name (here is Ubuntu_64bit)</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_3.png){: .center-image}
<em class="figure">Fig 3. Select a memory size based on your computer </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_4.png){: .center-image}
<em class="figure">Fig 4. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_5.png){: .center-image}
<em class="figure">Fig 5. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_6.png){: .center-image}
<em class="figure">Fig 6. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_7.png){: .center-image}
<em class="figure">Fig 7. Choose the VM file location. Default one is fine </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_8.png){: .center-image}
<em class="figure">Fig 8. Ubuntu_64bit is setup</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_9.png){: .center-image}
<em class="figure">Fig 9. Set installation iso file folder</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_10.png){: .center-image}
<em class="figure">Fig 10. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_11.png){: .center-image}
<em class="figure">Fig 11. </em>
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_12.png){: .center-image}
<em class="figure">Fig 12. Select ubuntu iso installation file</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_13.png){: .center-image}
<em class="figure">Fig 13. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_14.png){: .center-image}
<em class="figure">Fig 14. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_15.png){: .center-image}
<em class="figure">Fig 15. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_16.png){: .center-image}
<em class="figure">Fig 16. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_17.png){: .center-image}
<em class="figure">Fig 17. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_18.png){: .center-image}
<em class="figure">Fig 18. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_19.png){: .center-image}
<em class="figure">Fig 19. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_20.png){: .center-image}
<em class="figure">Fig 20. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_21.png){: .center-image}
<em class="figure">Fig 21. </em>
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_22.png){: .center-image}
<em class="figure">Fig 22. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_23.png){: .center-image}
<em class="figure">Fig 23. Make sure the installation file is removed. and put Enter to restart ubuntu</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_24.png){: .center-image}
<em class="figure">Fig 24. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_25.png){: .center-image}
<em class="figure">Fig 25. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_26.png){: .center-image}
<em class="figure">Fig 26. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_27.png){: .center-image}
<em class="figure">Fig 27. sudo apt-get update.</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_28.png){: .center-image}
<em class="figure">Fig 28. sudo apt-get install virtualbox-guest-utils</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_29.png){: .center-image}
<em class="figure">Fig 29. Create or select one folder in your windows os, which will be shared with Ubuntu.</em>



<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_30.png){: .center-image}
<em class="figure">Fig 30. Link the shared folder</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_31.png){: .center-image}
<em class="figure">Fig 31. </em>
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_32.png){: .center-image}
<em class="figure">Fig 32. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_33.png){: .center-image}
<em class="figure">Fig 33. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_34.png){: .center-image}
<em class="figure">Fig 34. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_35.png){: .center-image}
<em class="figure">Fig 35. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_36.png){: .center-image}
<em class="figure">
Fig 36. 
</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_37.png){: .center-image}
<em class="figure">Fig 37. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_38.png){: .center-image}
<em class="figure">Fig 38. Now you will see the shared files. And there has Anaconda install file for Ubuntu</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_39.png){: .center-image}
<em class="figure">Fig 39. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_40.png){: .center-image}
<em class="figure">Fig 40. Install Anaconda in Ubuntu</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_41.png){: .center-image}
<em class="figure">Fig 41. </em>
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_42.png){: .center-image}
<em class="figure">Fig 42. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_43.png){: .center-image}
<em class="figure">Fig 43. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_44.png){: .center-image}
<em class="figure">Fig 44. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_45.png){: .center-image}
<em class="figure">Fig 45. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_46.png){: .center-image}
<em class="figure">Fig 46. After installation, close terminal,and restart again. to make effective.</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_47.png){: .center-image}
<em class="figure">Fig 47. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_48.png){: .center-image}
<em class="figure">Fig 48. Install keras deep learning packages</em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_49.png){: .center-image}
<em class="figure">Fig 49. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_50.png){: .center-image}
<em class="figure">Fig 50. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_51.png){: .center-image}
<em class="figure">Fig 51. </em>
<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_52.png){: .center-image}
<em class="figure">Fig 52. </em>

<br>
![Clustering]({{ site.baseurl }}/assets/img/2019-11-01/ubuntu_vm_install_53.png){: .center-image}
<em class="figure">Fig 53. </em>

<hr class="with-margin">
<h4 class="header" id="quantization">Difference of Anaconda、conda、pip、virtualenv</h4>
If you have used pip and virtualenv in the past, you can use conda to perform all of the same operations. 
Pip is a package manager, and virtualenv is an environment manager; and conda is both.

Specifically, conda is a packaging tool and installer that aims to do more than what pip does; 
it handles library dependencies outside of the Python packages as well as the Python packages themselves. 
Conda also creates a virtual environment, like virtualenv does.

virtualenv is a tool to create isolated Python environments. Since Python 3.3, a subset of it has been integrated into the standard library under the venv module
pip is the reference Python package manager. It’s used to install and update packages. You’ll need to make sure you have the latest version of pip installed.

<hr class="with-margin">
### References

<ol>
  <li><a href="https://www.anaconda.com/distribution/">Anaconda</a></li>
  <li><a href="http://deeplearning.lipingyang.org/2018/12/23/anaconda-vs-miniconda-vs-virtualenv/">Anaconda vs. Miniconda vs. Virtualenv</a></li>
  <li><a href="https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/">Installing packages using pip and virtual environments</a></li>
  <li><a href="https://repo.continuum.io/archive/">Anaconda installer archive</a></li>
</ol>
