---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Hadoop_Hortonworks Sandbox HDP installation (Hadoop Part1)"
tags: ['Hortonworks Sandbox', 'HDP', 'Hadoop', 'spark', 'pig']
image: "hadoop/hadoop3.jpg"
identifier: 4
---

In this post, we're going to build environment about hadoop,big, spark. Finish Hortonworks Sandbox HDP installation. Later, we will use these system to finish some big data projects about using health data or other data.
<br> 
Author: Cell.

<!--more-->

<blockquote class="tip">
<strong>Hadoop_Hortonworks Sandbox:</strong> Apache Hadoop is an open source software platform for distributed storage and distributed processing of very large data sets on computer clusters built from commodity hardware.  Hadoop services provide for data storage, data processing, data access, data governance, security, and operations. More details could be check 
<a href="https://hortonworks.com/apache/hadoop/">Apache Hadoop</a>.
<a href="https://hortonworks.com/tutorial/hadoop-tutorial-getting-started-with-hdp/">Hadoop Tutorial – Getting Started with HDP</a>
and <a href="https://www.cloudera.com/downloads/hortonworks-sandbox.html">Hortonworks Sandbox</a>.
</blockquote>

<div class="list-of-contents">
  <h4>Post contents</h4>
  <ul></ul>
</div>

<hr class="with-margin">
<h4 class="header" id="intro">Download Hortonworks Sandbox</h4>

**Hortonworks Sandbox** The Sandbox is a straightforward, pre-configured, learning environment that contains the latest developments from Apache Hadoop, specifically the Hortonworks Data Platform (HDP). The Sandbox comes packaged in a virtual environment that can run in the cloud or on your personal machine.

**The Hortonworks Data Platform (HDP)** product includes Apache Hadoop and is used for storing, processing, and analyzing large volumes of data.

**Cloudera or Hortonworks** both comes with open source Apache Hadoop. However, Cloudera comes with vendor-lock management suite which helps in faster installation and deployment process. On the other hand, Hortonworks is 100% open source. As a result, Hortonworks updates come quicker than Cloudera.

Go to [Cloudera download webpage](https://www.cloudera.com/downloads.html).
![ClouderaWeb]({{ site.baseurl }}/assets/img/hadoop/hdp1_1.png){: .center-image}

<hr class="with-margin">
<h4 class="header" id="basic-implementation">Download the Hortonworks Sandbox</h4>

Find Hortonworks Sandbox, and click `Download the Hortonworks Sandbox`.
![ClouderaWeb_download]({{ site.baseurl }}/assets/img/hadoop/hadoop1_1.png){: .center-image}


<hr class="with-margin">
<h4 class="header" id="outro">Download</h4>
Then get this 
![ClouderaWeb_download]({{ site.baseurl }}/assets/img/hadoop/hadoop1_2.png){: .center-image}

Here, Installation Type is <strong>Virtualbox</strong>. Will also install Virtualbox in our computure later.

You need to register a account in Cloudera. After active your account, and login again, you will get download page.

![ClouderaWeb_download1]({{ site.baseurl }}/assets/img/hadoop/hadoop1_3.png){: .center-image}

![ClouderaWeb_version]({{ site.baseurl }}/assets/img/hadoop/hadoop1_4.png){: .center-image}


We could select HDP SANDBOX 3.0.1(LATEST).

<hr class="with-margin">
<h4 class="header" id="outro">VirtualBox</h4>


HDP Sandbox will run in VirtualBox. We could follow the link for VirtualBox in download page.
[Download VirtualBox](https://www.virtualbox.org/wiki/Downloads)
![ClouderaWeb_virtualbox]({{ site.baseurl }}/assets/img/hadoop/hadoop1_20.png){: .center-image}

<hr class="with-margin">
<h4 class="header" id="outro">FileZilla</h4>
We will use FileZilla (or  you may have yourown favorite FTP software.) to upload local file to Hadoop system.

The <strong>FileZilla</strong> Client not only supports FTP, but also FTP over TLS (FTPS) and SFTP. It is open source software distributed free of charge under the terms of the GNU General Public License.
[Download FileZilla](https://filezilla-project.org/download.php?platform=win64)
![ClouderaWeb_fileZillaPage]({{ site.baseurl }}/assets/img/hadoop/hadoop1_7.png){: .center-image}


<hr class="with-margin">
<h4 class="header" id="outro">PuTTY (only for Windows users)</h4>

For Mac or Ubuntu, Linux system, will use termial to login.
For win, we will use PuTTy to ssh login into Hadoop system. And most work will be done in terminal.

[Download PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)
![ClouderaWeb_putty]({{ site.baseurl }}/assets/img/hadoop/hadoop1_8.png){: .center-image}

<strong>Windows Terminal</strong> is a new, modern, fast, efficient, powerful, and productive terminal application for users of command-line tools and shells like Command Prompt, PowerShell, and WSL
[Windows Terminal](https://github.com/microsoft/Terminal)

So till now, we have VirtualBox, FileZilla. Win OS has putty installed.
![ClouderaWeb_softwareReady]({{ site.baseurl }}/assets/img/hadoop/hadoop1_6.png){: .center-image}

<hr class="with-margin">
<h4 class="header" id="outro">Start hortonworks Sandbox from VirtualBox</h4>
Import hortonworks Sandbox from VirtualBox. Need around 15min. Click File, then select Import.

![ClouderaWeb_softwareReady]({{ site.baseurl }}/assets/img/hadoop/hadoop1_12.png){: .center-image}

![ClouderaWeb_softwareReady]({{ site.baseurl }}/assets/img/hadoop/hadoop1_14.png){: .center-image}

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_16.png){: .center-image}
<br>
Setting, to make memory is more than 10GB if possible.

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_18.png){: .center-image}

Then click start in VirtualBox to inital and start Hortonworks. First boot will cost a little long time.

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_19.png){: .center-image}


<hr class="with-margin">
<h4 class="header" id="outro">Test HDP</h4>
After loading in VM VirtualBox.

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_22.png){: .center-image}

Also we could type localhost:1080 in webpage for usage, and login in dashboard and other functions. If you click 'Lauch dashbord‘ in the webpage, will be asked to login. We will discuss this later. 

Now, start PuTTy(windows). For Mac, Linux, Ubuntu, start terminal.

For Win:
![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_26.png){: .center-image}
type: 127.0.0.1 in host name, port is 2222. Click Open.

For terminal, type: ssh root@127.0.0.1 -p 2222

You will be asked to type user name.  root
password is hadoop
After this, you will be asked to reset password because this is the first initial time.
You can set one pwd as you want. Following screenshot, sudo passwd root, reset pws as hadoop.

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_27.png){: .center-image}

Then type ls, or cd.., ls

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_28.png){: .center-image}

Now you are in hadoop.

Let's type hdfs dfs -ls user/
this will check hdfs user folder

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_29.png){: .center-image}

Great!
Now start FileZilla, type in sftp://127.0.0.1, usernmae is root, password is hadoop, port is 2222.
You will see the same folders in hadoop. Notice: These folders or/and files are not under hdfs.

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_30.png){: .center-image}

<hr class="with-margin">
<h4 class="header" id="outro">Quit</h4>
Type exit in hadoop, puTTy will auto-close.
Then Close Hortonworks Sandbox vm. Click close. You do not need to save status. Just Power Off the machine.

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_32.png){: .center-image}

![ClouderaWeb_loginHdp]({{ site.baseurl }}/assets/img/hadoop/hadoop1_34.png){: .center-image}
Last step is close VirtualBox.

We will discuss upload data to hadoop, and creat database by Hive, and use pig, spark to do big data analyzing.

For Hive, will discuss database SQL knowledge.
For pig, will discuss SQL and Pig knowledge.
For spark, will discuss pyspark and python, java knowledge.
Enjoy our journey. 

If you have any suggestion or comments, or any question, please email me.


### References

<ol>
  <li><a href="https://hortonworks.com/tutorial/hadoop-tutorial-getting-started-with-hdp/">Apache Hadoop</a></li>
  <li><a href="https://www.cloudera.com/downloads/hortonworks-sandbox.html">Hortonworks Sandbox</a></li>
  <li><a href="https://hortonworks.com/apache/hadoop/">Hadoop Tutorial – Getting Started with HDP</a></li>
</ol>
