---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Azure HDInsight - Hadoop, Spark, & Kafka Service"
tags: ['Azure', 'HDInsight', 'Hadoop', 'Spark']
image: "2020-01-21/hdinsight-architecture-iot.png"
identifier: 3
---
Azure HDInsight is easy, cost-effective, enterprise-grade service for open source analytics. Azure HDInsight is a managed, full-spectrum, open-source analytics service in the cloud for enterprises. You can use open-source frameworks such as Hadoop, Apache Spark, Apache Hive, LLAP, Apache Kafka, Apache Storm, R, and more.
Author and collect by: Sheryl

<!--more-->

<blockquote class="tip">
 <strong>Azure HDInsight</strong>  is a cloud distribution of Hadoop components. Azure HDInsight makes it easy, fast, and cost-effective to process massive amounts of data. You can use the most popular open-source frameworks such as Hadoop, Spark, Hive, LLAP, Kafka, Storm, R, and more. With these frameworks, you can enable a broad range of scenarios such as extract, transform, and load (ETL), data warehousing, machine learning, and IoT.
 
 
 Check <a href="https://docs.microsoft.com/en-us/azure/hdinsight/hdinsight-component-versioning">Hadoop technology stack components</a> on HDInsight.
Check <a href="https://azure.microsoft.com/en-us/services/hdinsight/">Hadoop in HDInsight</a> 
</blockquote>

<div class="list-of-contents">
  <h4>Post contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization"> Create Apache Hadoop cluster in Azure HDInsight using Azure</h4>

Sign in to the Azure Stack Hub portal.

![azureservice]({{ site.baseurl }}/assets/img/2020-01-21/portal-1.png){: .center-image}
<em class="figure">Fig Login and go to Portal.
</em>
<br>



![azureservice]({{ site.baseurl }}/assets/img/2020-01-21/portal-2.png){: .center-image}
<em class="figure">Fig Create a new resource.
</em>
<br>


To create new resource.
![azureservice]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-1.png){: .center-image}
<em class="figure">Fig 1. Find Analytics->Azure HDInsight.
</em>
<br>

 
Go into project details.
![VM]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-2.png){: .small70-image}
<em class="figure">Fig 2. project details</em>
<br>

<strong>resource group</strong> - A container that holds related resources for an Azure solution. The resource group includes those resources that you want to manage as a group. You decide which resources belong in a resource group based on what makes the most sense for your organization.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/scope-levels.png.png){: .center-image}

Check more details about <a href="https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview">Resource</a>.


Cluster details. select/create a resource group, cluster details and credentials.
Here we select Hadoop as cluster type.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-3.png){: .center-image}
<em class="figure">Fig 3. Cluster details.</em>
<br>

Select the <strong> Next: Storage >> </strong> to advance to the storage settings.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-4.png){: .center-image}
<em class="figure">Fig 4. Cluster details. </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-5.png){: .center-image}
<em class="figure">Fig 5. Storage details</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-6.png){: .center-image}
<em class="figure">Fig 6. Security and networking details</em>
<br>

After vm selections, review all details. 

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-7.png){: .center-image}
<em class="figure">Fig 7. Configuration </em>
<br>
You could download a template for automation, or could download after creating cluster.

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-8.png){: .small70-image}
<em class="figure">Fig 8.Review.</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-9.png){: .center-image}
<em class="figure">Fig 9.Review  and click create </em>
<br>

After click create, will deployment progress.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-10.png){: .small70-image}
<em class="figure">Fig 10. deployment progress</em>
<br>

After deployment is complete, you could download deployment details, got to resource.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-12.png){: .small70-image}
<em class="figure">Fig 11. deployment is complete </em>
<br>

Go to Dashboard to check all resource created.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-13a.png){: .small70-image}
<em class="figure">Fig 12a. check All resources</em>
<br>

Click one resource, here is hdinsight1. there is a <strong> URL</strong>  at the right, copy paste to browser.

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-13b.png){: .center-image}
<em class="figure">Fig 12b. Check resource details,and will connect.</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-13c.png){: .center-image}
<em class="figure">Fig 12c. Fill credentials when you type in creating this.</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-13.png){: .center-image}
<em class="figure">Fig 12d. Now, you will see dashboard of hadoop.</em>
<br>

Now, we will use SSH to login depend on your requirements.

If you're using the Azure Stack Development Kit (ASDK), you might not have access to a Secure Shell (SSH) client. If you need a client, several packages include an SSH client. For example, PuTTY includes an SSH client and SSH Key Generator (puttygen.exe). 
<a href="https://docs.microsoft.com/en-us/azure-stack/user/azure-stack-dev-start-howto-ssh-public-key?view=azs-2002">Use an SSH public key</a>. 
<a href="https://www.putty.org/">Download PuTTY</a>. 

Then will try to login. Here is using PuTTY for windows, for Mac, please check fig 17.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-14.png){: .center-image}
<em class="figure">Fig 13. Use PuTTY (windows) to login</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-15.png){: .center-image}
<em class="figure">Fig 13b. Use PuTTY (windows) to login</em>
<br>


![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/hdinsight-16.png){: .center-image}
<em class="figure">Fig 13c. now you are in</em>
<br>

For Mac, or Linux
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/azure-ssh1.png){: .center-image}
<em class="figure">Fig 14. Terminal to login.</em>
<br>

Type login name and pwd
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/azure-ssh2.png){: .center-image}
<em class="figure">Fig 15.</em>
<br>

Here you go.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-21/azure-ssh3.png){: .center-image}
<em class="figure">Fig 15.</em>
<br>

You can also run Apache Hive queries.

<strong>Apache Hive</strong> is the most popular component used in HDInsight. There are many ways to run Hive jobs in HDInsight. In this quickstart, you use the Ambari Hive view from the portal. For other methods for submitting Hive jobs, check <a href="https://docs.microsoft.com/en-us/azure/hdinsight/hadoop/hdinsight-use-hive">Use Hive in HDInsight</a>.

<hr class="with-margin">
### References

<ol>

<li><a href="https://docs.microsoft.com/en-us/azure/hdinsight/hdinsight-overview">What is Azure HDInsight?</a></li>

  <li><a href="https://docs.microsoft.com/en-us/azure/hdinsight/hadoop/apache-hadoop-linux-create-cluster-get-started-portal">Create Apache Hadoop cluster in Azure HDInsight using Azure portal</a></li>
  
  <li><a href="https://docs.microsoft.com/en-us/azure/hdinsight/hdinsight-component-versioning"> What are the Apache Hadoop components and versions available with HDInsight</a></li>
  
</ol>
