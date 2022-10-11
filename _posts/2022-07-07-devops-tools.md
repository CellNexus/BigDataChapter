---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "DevOps Tools"
tags: ['DevOp', 'Tools', 'agents']
image: "2022-07-07/devops-tools-logo.png"
identifier: 3
---
DevOps Tool is an application that helps automate the software development process. It mainly focuses on communication and collaboration between product management, software development, and operations professionals. DevOps tool also enables teams to automate most of the software development processes like build, conflict management, dependency management, deployment, etc. and helps reduce manual efforts.

Author and collect by: Cell

<!--more-->

<blockquote class="tip">

The <strong> Azure DevOps</strong>service is one such SaaS offering that offers a fully featured DevOps platform consisting of: Azure Boards (Planning and Management of the Project), Azure Pipelines (CI/CD Pipeline), Azure Repos (Cloud-hosted private Git Repositories), Azure Test Plans (Manual and Exploratory testing tools),Azure Artifacts (Artifact Storage).

<strong>Agent</strong> is a server with the appropriate Operating System and the tools installed and configured. Azure DevOps supports the following two types of Agents

<strong>Microsoft Hosted Agent</strong> – These agents are managed by Microsoft.
<strong>Self-Hosted Agents</strong> – These are created and managed by the Customer.

</blockquote>

<div class="list-of-contents">
  <h4>Contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization">Azure Pipelines</h4>

Azure Pipelines automatically builds and tests code projects to make them available to others. It works with just about any language or project type. Azure Pipelines combines continuous integration (CI) and continuous delivery (CD) to test and build your code and ship it to any target.
<br>
Continuous Integration (CI) is the practice used by development teams of automating merging and testing code. Implementing CI helps to catch bugs early in the development cycle, which makes them less expensive to fix. Automated tests execute as part of the CI process to ensure quality. Artifacts are produced from CI systems and fed to release processes to drive frequent deployments. The Build service in Azure DevOps Server helps you set up and manage CI for your applications.
<br>
Continuous Delivery (CD) is a process by which code is built, tested, and deployed to one or more test and production environments. Deploying and testing in multiple environments increases quality. CI systems produce deployable artifacts, including infrastructure and apps. Automated release processes consume these artifacts to release new versions and fixes to existing systems. Monitoring and alerting systems run continually to drive visibility into the entire CD process.
<br>
Continuous Testing (CT) on-premises or in the cloud is the use of automated build-deploy-test workflows, with a choice of technologies and frameworks, that test your changes continuously in a fast, scalable, and efficient manner.
<br>



![db]({{ site.baseurl }}/assets/img/2022-04-08/pipeline-view.png){: .small70-image}
<em class="figure">Fig. Key concepts overview</em>
<br>


<hr class="with-margin">
<h4 class="header" id="quantization">Agent</h4>

<br>
When your build or deployment runs, the system begins one or more jobs. An agent is computing infrastructure with installed agent software that runs one job at a time. For example, your job could run on a Microsoft-hosted Ubuntu agent.
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Self-hosted macOS agents</h4>

To build and deploy Xcode apps or Xamarin.iOS projects, you'll need at least one macOS agent. This agent can also build and deploy Java and Android apps.
<br>


<strong> Step 1: enable agent machine permission for terminal</strong>
<br>
spctl developer-mode enable-terminal
<br>

<br>
Then in Settings -> Security & Privacy -> Developer Tools
<br>
unlock
<br>
set the tick on "Terminal"
<br>

![permission1]({{ site.baseurl }}/assets/img/2022-04-08/0a1.png){: .small70-image}
<em class="figure">Fig . OS permission.</em>
<br>

![permission1]({{ site.baseurl }}/assets/img/2022-04-08/0a2.png){: .small70-image}
<em class="figure">Fig . OS permission.</em>
<br>
<br>

<strong> Step 2: Generate and Copy Authenticate with a personal access token (PAT) from Azure DevOps</strong>

Sign in with the user account you plan to use in your Azure DevOps organization.
<br>
From your home page, open your user settings, and then select Personal access tokens.
<br>
For the scope select <strong>Agent Pools (read, manage) </strong>and make sure all the other boxes are cleared. If it's a deployment group agent, for the scope select <strong>Deployment group </strong>(read, manage) and make sure all the other boxes are cleared.
<br>
![pat]({{ site.baseurl }}/assets/img/2022-04-08/1a1.png){: .small70-image}
<em class="figure">Fig . PAT.</em>
<br>

![pat]({{ site.baseurl }}/assets/img/2022-04-08/1a2.png){: .small70-image}
<em class="figure">Fig . PAT.</em>
<br>
<br>

<strong> Step 3: Install package on agent machine</strong>


![pat]({{ site.baseurl }}/assets/img/2022-04-08/2a1.png){: .small70-image}
<em class="figure">Fig . PAT.</em>
<br>
<br>

Download the tar file: xattr -c vsts-agent-osx-x64-V.v.v.tar.gz.
<br>
Unpack the agent into the directory of your choice. cd to that directory and run ./config.sh. Make sure that the path to the directory contains no spaces because tools and scripts don't always properly escape spaces.

<br>

![agent]({{ site.baseurl }}/assets/img/2022-04-08/3a0.png){: .small70-image}
<em class="figure">Fig . Download and prepare tar files.</em>
<br>
<br>
![agent]({{ site.baseurl }}/assets/img/2022-04-08/3a1.png)
<em class="figure">Fig . Agent Config.</em>
<br>
<br>
![agent]({{ site.baseurl }}/assets/img/2022-04-08/3a2.png){: .small70-image}
<em class="figure">Fig . Agent Config.</em>
<br>
<br>

Configurations:
<br>
Server URL: Azure Pipelines: https://dev.azure.com/{your-organization}
<br>
Authentication type: PAT
<br> 
Default others or set your work directory.

<strong> Step 4: Start </strong>

![runagent]({{ site.baseurl }}/assets/img/2022-04-08/4a1.png)
<em class="figure">Fig . Run Agent .</em>
<br>
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Check Agent on AZ DevOps </h4>


<br>

![runagent]({{ site.baseurl }}/assets/img/2022-04-08/5a1.png){: .small70-image}
<em class="figure">Fig . Go to Agent Poll.</em>
<br>
<br>

![runagent]({{ site.baseurl }}/assets/img/2022-04-08/5a2.png){: .small70-image}
<em class="figure">Fig . Add Agent .</em>
<br>
<br>

![runagent]({{ site.baseurl }}/assets/img/2022-04-08/5a3.png){: .small70-image}
<em class="figure">Fig . Check Agent .</em>
<br>
<br>

![runagent]({{ site.baseurl }}/assets/img/2022-04-08/5a5.png){: .small70-image}
<em class="figure">Fig . Check Agent capabilities.</em>
<br>
<br>

<hr class="with-margin">

### References

<ol>
  <li><a href="https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/agents?view=azure-devops&tabs=browser">Azure Pipelines agents</a></li>
</ol>

<ol>
  <li><a href="https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/v2-osx?view=azure-devops">Self-hosted macOS agents</a></li>
</ol>

<ol>
  <li><a href="https://docs.microsoft.com/en-us/azure/devops/pipelines/build/variables?view=azure-devops&tabs=yaml">Pipeline variables</a></li>
</ol>

<hr class="with-margin">

![go]({{ site.baseurl }}/assets/img/2022-04-08/selfhostagent-case1.png){: .autofit-image}
<br>