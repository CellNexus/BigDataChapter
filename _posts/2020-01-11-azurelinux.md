---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Azure - create Linux server"
tags: ['Azure', 'Linux', 'Server']
image: "2020-01-11/azure-images.png"
identifier: 3
---
Azure supports common Linux distributions, including Red Hat, SUSE, Ubuntu, CentOS, Debian, Oracle Linux and CoreOS. We can selecet Azure to create Linux virtual machines (VMs), deploy and run containers in Kubernetes, or other files.

Author and collect by: Sheryl

<!--more-->

<blockquote class="tip">
 <strong>Microsoft Azure</strong> is a cloud computing service created by Microsoft for building, testing, deploying, and managing applications and services through Microsoft-managed data centers.On-premises, hybrid, multicloud or at the edge – anyone can create secure, future-ready solutions:
   <ol>    
    <li>
      AI + machine learning
    </li>
    <li>
      Compute
    </li>
    <li>
	Containers
	</li>
    <li>
	Internet of Things (IoT)
	</li>
	<li>
      Get an Azure <a href="https://azure.microsoft.com/">free account</a>.
    </li>
  </ol>
</blockquote>

<div class="list-of-contents">
  <h4>Post contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization">Create Linux Red Hat service on Azure</h4>

First, we have a Azure account, and login. Sign in to the Azure Stack Hub portal.

After login, go All, you will see general services here. You also could do a service serach at the left-top All service search engine.  Here we select Free Services.

![azureservice]({{ site.baseurl }}/assets/img/2020-01-11/1.png){: .center-image}
<em class="figure">Fig 1. Azure service selection.
</em>
<br>

There are some free service provided by Azure free account. 
We could select to create a Windows VM or Linux VM, or other service.  
Here we choose Linux VM for a future server.

![VM]({{ site.baseurl }}/assets/img/2020-01-11/2.png){: .small70-image}
<em class="figure">Fig 2. Free Services interface for the Azure free account</em>
<br>

Here we will build our vm by selecting details.
We need to create a new Resouce group or select one exist one for this vm
Define VM name, and select Region. For Region, we could select the closest one.
you could choose linux os, like Red Hat Enterprise Linux 7.4 is for this vm. Here choose CoreOS, Also it is free.

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/3.png){: .center-image}
<em class="figure">Fig 3. Create a virtual machine.</em>
<br>

<strong>resource group</strong> - A container that holds related resources for an Azure solution. The resource group includes those resources that you want to manage as a group. You decide which resources belong in a resource group based on what makes the most sense for your organization.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/scope-levels.png.png){: .center-image}

Check more details about <a href="https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview">Resource</a>.


![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/4.png){: .center-image}
<em class="figure">Fig 4. Create a new resource group. </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/5.png){: .center-image}
<em class="figure">Fig 5. VM details </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/8.png){: .center-image}
<em class="figure">Fig 6. SSH</em>
<br>

After vm selections, review all details. 

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/9.png){: .center-image}
<em class="figure">Fig 7. </em>
<br>
You could download a template for automation, or could download after create this vm.

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/10.png){: .small70-image}
<em class="figure">Fig 8.Template.</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/11.png){: .center-image}
<em class="figure">Fig 9.Template zip file </em>
<br>

After click create, will deployment progress.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/13.png){: .small70-image}
<em class="figure">Fig 10. deployment progress</em>
<br>

After deployment is complete, you could download deployment details, got to resource.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/14.png){: .small70-image}
<em class="figure">Fig 11. deployment is complete </em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/15.png){: .small70-image}
<em class="figure">Fig 12. REsource details</em>
<br>
If you're using the Azure Stack Development Kit (ASDK), you might not have access to a Secure Shell (SSH) client. If you need a client, several packages include an SSH client. For example, PuTTY includes an SSH client and SSH Key Generator (puttygen.exe). 
<a href="https://docs.microsoft.com/en-us/azure-stack/user/azure-stack-dev-start-howto-ssh-public-key?view=azs-2002">Use an SSH public key</a>. 
<a href="https://www.putty.org/">Download PuTTY</a>. 

Then will try to login. Here is using PuTTY for windows, for Mac, please check fig 17.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/16.png){: .center-image}
<em class="figure">Fig 13. Use PuTTY (windows) to login</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/17.png){: .center-image}
<em class="figure">Fig 14. Import SSH which is used for Azure pk.</em>
<br>

Type login name and pwd
![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/18.png){: .center-image}
<em class="figure">Fig 15. Import SSH which is used for Azure pk.</em>
<br>


![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/19.png){: .center-image}
<em class="figure">Fig 16. Login.</em>
<br>

Or you can get Connect file and details about ssh.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/20.png){: .small70-image}
<em class="figure">Fig 17. Select vm,and click Connect tab.</em>
<br>

![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/21.png){: .center-image}
<em class="figure">Fig 18. Connect via SSH with client.</em>
<br>

For windows VM, you also could download RDP file, to directly connect with your vm.
![Clustering]({{ site.baseurl }}/assets/img/2020-01-11/22.png){: .center-image}
<em class="figure">Fig 18. Connect via RDP.</em>
<br>


<hr class="with-margin">
### References

<ol>
  <li><a href="https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/overview">What is Azure Resource Manager</a></li>
  <li><a href="https://docs.microsoft.com/en-us/azure-stack/user/azure-stack-quick-linux-portal?view=azs-2002"> Create a Linux server VM by using the Azure Stack Hub portal</a></li>
  <li><a href="https://docs.microsoft.com/en-us/learn/modules/create-linux-virtual-machine-in-azure/">Learn Module: Create a Linux virtual machine in Azure</a></li>
</ol>
