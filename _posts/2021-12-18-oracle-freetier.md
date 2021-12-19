---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Oracle Cloud Infrastructure Always Free services"
tags: ['Oracle', 'Cloud', 'Free tier', 'Always free']
image: "2021-12-18/oracle-alwaysfree-1.jpeg"
identifier: 3
---
Oracle began offering Always Free services including Compute, Storage, and Autonomous Database. The newest Always Free services include Ampere A1 Compute, Autonomous JSON Database, NoSQL, APEX Application Development, Logging, Service Connector Hub, Application Performance Monitoring (APM), flexible load balancer, flexible network load balancer, VPN Connect V2, Oracle Security Zones, Oracle Security Advisor, and OCI Bastion, making Oracle’s Always Free portfolio of services and resources among the most generous in the industry. 

Author and collect by: Cell

<!--more-->

<blockquote class="tip">
Oracle builds out their portfolio of <strong> Oracle Cloud </strong> Infrastructure Always Free services.  

Compute resources: Oracle offers the most significant Always Free Arm resources (four OCPUs, 24-GB Memory) in the industry to enable developers to build and test meaningful apps.

New Always Free includes: Databases resources and services (2 Autonomous Databases, 20 GB each), application development services, Observability and Management resources and services, Infrastructure and Networking services, Security resources and others.

Here we focus on Compute resources which could be used for your webiste, wordpress website and others.

</blockquote>

<div class="list-of-contents">
  <h4>Contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization">Aim</h4>
Following screenshots show Oracle Cloud services. There are "Always Free Eligible" for Always Free tier.

Here, we are going to create one compute instance VM.

![freetier1]({{ site.baseurl }}/assets/img/2021-12-18/oracle-free-0.png){: .small70-image}
<em class="figure">Fig. Oracle Cloud Resources 1</em>
<br>

![freetier2]({{ site.baseurl }}/assets/img/2021-12-18/oracle-free-a.png){: .small70-image}
<em class="figure">Fig. Oracle Cloud Resources 2</em>
<br>


<hr class="with-margin">
<h4 class="header" id="quantization">Step 1: Create a VM instance</h4>

<br>
Login Oracle Cloud
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-login.png){: .small70-image}
<em class="figure">Fig . Oracle Cloud Login.</em>
<br>

Quickstarts Launch Resources
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-1.png){: .small70-image}
<em class="figure">Fig . Launch Resources -  Create a VM instance.</em>
<br>


<hr class="with-margin">
<h4 class="header" id="quantization">Step 2: Create compute instance </h4>

Create compute instance (Always free)
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-2a.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance.</em>
<br>


Shape VM Image
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-2c.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : Image and shape</em>
<br>



Shape VM Image
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-2b.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : shape</em>
<br>

Browse all images
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-2d.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : image choices</em>
<br>



Here is using Oracle Linux and set version as 8.
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-2e.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : image choices</em>
<br>


Here is using Ampere.
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-2f.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : Ampere image</em>
<br>


4 OCPUs, and 24M RAM.
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-2g.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : OCPU and Memory setting</em>
<br>


VM instance review.
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-2h.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : VM instance review</em>
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Step 3: set SSH</h4>

Add SSH pub key to VM instance. Check previous blog to get pub key when using win, macos or Linux.

like macos:  '''cat .ssh/id_rsa.pub'''


![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-4.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : set SSH</em>
<br>


![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-4a.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : set SSH</em>
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Step 4: create VM.</h4>

Create
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-5.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : create VM</em>
<br>


<hr class="with-margin">
<h4 class="header" id="quantization">Step 5: VM is created.</h4>

VM is created. Check status.
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-6.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : creating VM</em>
<br>

VM is created. Running.
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-8.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : VM is running</em>
<br>



<hr class="with-margin">
<h4 class="header" id="quantization">Step 6: Testing VM and make a connection.</h4>

'''ssh name@vmip'''
<br>

![createvm]({{ site.baseurl }}/assets/img/2021-12-18/oracle-9a.png){: .small70-image}
<em class="figure">Fig . Configure a VM instance : VM is accessed</em>
<br>

Done
<br>


We will post how to deploy wordpress or host mysql-API-docker images in Oracle Cloud using always free tier.
<br>

<hr class="with-margin">
### References

<ol>
  <li><a href="https://blogs.oracle.com/cloud-infrastructure/post/oracle-builds-out-their-portfolio-of-oracle-cloud-infrastructure-always-free-services">Oracle builds out their portfolio of Oracle Cloud Infrastructure Always Free services</a></li>
</ol>

<ol>
  <li><a href="https://docs.oracle.com/en-us/iaas/Content/FreeTier/freetier.htm">Oracle Cloud Infrastructure Free Tier</a></li>
</ol>

<ol>
  <li><a href="https://docs.oracle.com/en-us/iaas/Content/FreeTier/freetier_topic-Always_Free_Resources.htm">Always Free Resources</a></li>
</ol>

<hr class="with-margin">

![oracleCloud]({{ site.baseurl }}/assets/img/2021-12-18/Oracle-Cloud.png){: .autofit-image}
<br>