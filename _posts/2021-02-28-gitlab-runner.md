---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Set up gitlab-runner for GitLab CI"
tags: ['GitHub', 'CI/CD']
image: "2021-02-28\runner_logo.png"
identifier: 3
---
Using your local development machine as GitLab CI runner instead of the shared runners. GitLab runner is a build instance which is used to run the jobs over multiple machines and send the results to GitLab and which can be placed on separate users, servers, and local machine. You can register the runner as shared or specific after installing it. 

Author and collect by: Sheryl, Cell

<!--more-->

<blockquote class="tip">
 In GitLab CI/CD, <strong>runners</strong> run the code defined in .gitlab-ci.yml. A runner is a lightweight, highly-scalable agent that picks up a CI job through the coordinator API of GitLab CI/CD, runs the job, and sends the result back to the GitLab instance.

Runners are created by an administrator and are visible in the GitLab UI. Runners can be specific to certain projects or available to all projects.

</blockquote>

<div class="list-of-contents">
  <h4>Contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization">Aim</h4>
Registering runners by using VPS. Here is using VM. This VM could be created from Azure, AWS, GCP or any providers. Here VM is using ubuntu 20.04.

<hr class="with-margin">
<h4 class="header" id="quantization">Step 1: Create gitlab-runner</h4>

#ssh root@your_server_ip_address

#adduser gitlab-runner

May sign permissions to this user without add sudo (like adding gitlab-runner ALL=(ALL) NOPASSWD:ALL), and offer docker permissions depend on your arch).

![createuser]({{ site.baseurl }}/assets/img/2021-02-28/1.png){: .center-image}
<em class="figure">Fig 1. Create gitlab-runner user.</em>
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Step 2: Install runner/h4>

[Installing GitLab Runner](https://docs.gitlab.com/runner/install/linux-repository.html)
![installrunner]({{ site.baseurl }}/assets/img/2021-02-28/3.png){: .center-image}
<em class="figure">Fig 2. Install Gitlab runner.</em>
<br>

![installrunner]({{ site.baseurl }}/assets/img/2021-02-28/5.png){: .center-image}
<em class="figure">Fig 3. Install Gitlab runner.</em>
<br>

1 Add the official GitLab repository:

curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash

![installrunner]({{ site.baseurl }}/assets/img/2021-02-28/4.png){: .center-image}
<em class="figure">Fig 4. Install Gitlab runner.</em>
<br>

2 Install the latest version of GitLab Runner

export GITLAB_RUNNER_DISABLE_SKEL=true; sudo -E apt-get install gitlab-runner

![installrunner]({{ site.baseurl }}/assets/img/2021-02-28/6.png){: .center-image}
<em class="figure">Fig 5. Install Gitlab runner.</em>
<br>


<hr class="with-margin">
<h4 class="header" id="quantization">Step 3: Registering runners</h4>
Registering a runner is the process that binds the runner with a GitLab instance.
[Registering runners](https://docs.gitlab.com/runner/register/)

![regesterrunner]({{ site.baseurl }}/assets/img/2021-02-28/7.png){: .center-image}
<em class="figure">Fig 6. Register runner Linux</em>
<br>

sudo gitlab-runner register

![regesterrunner]({{ site.baseurl }}/assets/img/2021-02-28/8.png){: .center-image}
<em class="figure">Fig 7. Register runner with your CICD setting info</em>
<br>
Enter your GitLab instance URL (also known as the gitlab-ci coordinator URL).

Enter the token you obtained to register the runner.

Enter a description for the runner. You can change this value later in the GitLab user interface.

Enter the tags associated with the runner, separated by commas. You can change this value later in the GitLab user interface.

Provide the runner executor. For most use cases, enter docker.

If you entered docker as your executor, you’ll be asked for the default image to be used for projects that do not define one in .gitlab-ci.yml.

<strong>tag</strong> should be the same as your cicd file.
![regesterrunner]({{ site.baseurl }}/assets/img/2021-02-28/9.png){: .center-image}
<em class="figure">Fig 8. Register runner with your CICD setting info</em>
<br>


here select <strong>shell</strong> type.
![regesterrunner]({{ site.baseurl }}/assets/img/2021-02-28/11.png){: .center-image}
<em class="figure">Fig 9. Register runner with your CICD setting info</em>
<br>



<hr class="with-margin">
<h4 class="header" id="quantization">Step 4: Check runner in gitlab setting cicd runner</h4>
Now your own runner is ready for fire pipeline.

![gitaction11]({{ site.baseurl }}/assets/img/2021-02-28/12.png){: .center-image}
<em class="figure">Fig 10. Available runner.</em>
<br>



<hr class="with-margin">
### References

<ol>
  <li><a href="https://docs.gitlab.com/ee/ci/runners/">Configuring runners in GitLab</a></li>
</ol>

<ol>
  <li><a href="https://docs.gitlab.com/runner/register/">Registering runners</a></li>
</ol>

<ol>
  <li><a href="https://docs.gitlab.com/runner/configuration/advanced-configuration.html">Advanced configuration</a></li>
</ol>

<hr class="with-margin">

![gitaction8]({{ site.baseurl }}/assets/img/2021-02-28/gitlab-runner-pipeline.png){: .autofit-image}
<br>