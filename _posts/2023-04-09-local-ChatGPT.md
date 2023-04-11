---
layout: post
category: blog
permalink: /:categories/:year/:month/:day/:title
title: "Build local ChatGPT-like by using LLaMa and Alpaca"
tags: ['ChatBot', 'ChatGPT', 'LLaMa', 'Alpaca']
image: "2023-04-09/logo1.png"
identifier: 3
---
"Stanford Alpaca" is a research project developed by a team at Stanford University's Natural Language Processing Group, and "LLaMA" stands for "Language Learning for Instruction Following by Matching and Attention.".

Author and collect by: Cell

<!--more-->
<blockquote class="tip">

<strong>The Stanford Alpaca model </strong>is an AI language model designed to follow instructions and perform tasks based on natural language input. It is based on the Transformer architecture, which is similar to the one used by ChatGPT. However, the Alpaca model is specifically designed to perform instruction-following tasks, such as following recipes or assembling furniture


</blockquote>

<div class="list-of-contents">
  <h4>Contents</h4>
  <ul></ul>
</div>


<hr class="with-margin">
<h4 class="header" id="quantization">What is Stanford Alpaca</h4>
<br>
"Stanford Alpaca" is a research project developed by a team at Stanford University's Natural Language Processing Group, and "LLaMA" stands for "Language Learning for Instruction Following by Matching and Attention."
<br>
The Stanford Alpaca model is an AI language model designed to follow instructions and perform tasks based on natural language input. It is based on the Transformer architecture, which is similar to the one used by ChatGPT. However, the Alpaca model is specifically designed to perform instruction-following tasks, such as following recipes or assembling furniture.
<br>
The Alpaca model uses a combination of language modeling, attention mechanisms, and imitation learning to generate natural language responses and perform tasks. It was trained on a large corpus of instructional text and can generalize to new instructions and tasks.
<br>
Overall, the Stanford Alpaca model is a specialized language model designed for a specific task, while ChatGPT is a more general language model that can be used for a wide range of natural language processing tasks
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">VS. ChatGPT</h4>

<br>
The main difference between the Stanford Alpaca model and ChatGPT is their purpose and focus. The Alpaca model is designed specifically for instruction-following tasks, while ChatGPT is a general-purpose language model that can be used for a wide range of tasks.
<br>
The Alpaca model is trained on a large corpus of instructional text and can perform tasks such as following recipes or assembling furniture. It uses a combination of language modeling, attention mechanisms, and imitation learning to generate natural language responses and perform tasks.
<br>
On the other hand, ChatGPT is a more general-purpose language model that can be used for a wide range of natural language processing tasks, such as question-answering, text completion, summarization, and more. It is based on the Transformer architecture and is trained on a large corpus of text from the internet.
<br>
While both the Stanford Alpaca model and ChatGPT use natural language processing techniques to generate natural language responses, their focus and training data are different. The Alpaca model is specialized for instruction-following tasks, while ChatGPT is designed for more general language tasks.
<br>
<hr class="with-margin">
<h4 class="header" id="quantization">how was it trained</h4>

<br>
Alpaca is fine-tuned on LLaMa, Meta’s large language model which recently leaked online. And to train this language model, scientists used OpenAI’s “text-davinci-003” model to generate 52K high-quality self-instruction data. With this dataset, they fine-tuned the LLaMA model using HuggingFace’s training framework and released the Alpaca 7B. You can also use Meta’s LLaMA model, but in my testing, Stanford’s Alpaca LLM performed much better and it’s also quite fast.
<br>

![db]({{ site.baseurl }}/assets/img/2022-04-09/1.png){: .small70-image}
<em class="figure">Fig. Model</em>

<hr class="with-margin">
<h4 class="header" id="quantization">Dalai:Run LLaMA and Alpaca on your computer</h4>

<br>
Introducing <strong>Dalai</strong> a super simple way to run LLaMA AI on your computer. 
<br>
No need to bother building cpp files, cloning github, and downloading files and stuff. Everything is automated.  
<br>
All you need is: "npx dalai llama"
<br>
[Website](https://cocktailpeanut.github.io/dalai)
<br>

<hr class="with-margin">
<h4 class="header" id="quantization">Build Steps</h4>

<strong> Requirements </strong>
Git
<br>
Docker engine
<br>
Docker composer
<br>

<strong> Step 1: </strong>

```
git clone https://github.com/cocktailpeanut/dalai.git
```

<br>

![db]({{ site.baseurl }}/assets/img/2022-04-09/2.png){: .small70-image}
<em class="figure">Fig. Git Clone 1</em>

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/3.png){: .small70-image}
<em class="figure">Fig. Git Clone 2</em>


<br>
<strong> Step 2: </strong>

```
cd dalai
```

```
docker compose build
```

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/4.png){: .small70-image}
<em class="figure">Fig. docker compose build</em>

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/5.png){: .small70-image}
<em class="figure">Fig. docker compose build</em>

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/6.png){: .small70-image}
<em class="figure">Fig. docker compose build</em>


```
docker compose run dalai npx dalai alpaca install 7B
```

<br>
Notes: change alpaca to 'llama', and '7B' by other another model
<br>
There are no 30B and 65B Alpaca models.
<br>
Downloaded model goes in './models'
<br>

![db]({{ site.baseurl }}/assets/img/2022-04-09/7.png){: .small70-image}
<em class="figure">Fig. 7B</em>
<br>

![db]({{ site.baseurl }}/assets/img/2022-04-09/8.png){: .small70-image}
<em class="figure">Fig. install model</em>
<br>

![db]({{ site.baseurl }}/assets/img/2022-04-09/9.png){: .small70-image}
<em class="figure">Fig. install model</em>
<br>

![db]({{ site.baseurl }}/assets/img/2022-04-09/10.png){: .small70-image}
<em class="figure">Fig. docker ps -a</em>
<br>

```
docker compose up -d
```

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/11.png){: .small70-image}
<em class="figure">Fig. docker ps</em>
<br>

Open web browser, open: http://127.0.0.1:3000/ or http://localhost:3000

```
http://localhost:3000
```

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/12.png){: .small70-image}
<em class="figure">Fig. web ui</em>
<br>

Check models

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/12b.png){: .small70-image}
<em class="figure">Fig. only one model</em>
<br>


<hr class="with-margin">
<h4 class="header" id="quantization">Install other models</h4>

Install other models, here are llama 7B 13B (may need around 1hour)

```
docker compose run dalai npx dalai llama install 7B 13B
```

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/13.png){: .small70-image}
<em class="figure">Fig. install models</em>
<br>

<br>
![db]({{ site.baseurl }}/assets/img/2022-04-09/14.png){: .small70-image}
<em class="figure">Fig. install models</em>
<br>


```
docker compose up -d
```

then

```
http://localhost:3000
```

<hr class="with-margin">
<h4 class="header" id="quantization">Testing</h4>



<hr class="with-margin">

### References

<ol>
  <li><a href="https://github.com/cocktailpeanut/dalai">Dalai:Run LLaMA and Alpaca on your computer.</a></li>
</ol>

<ol>
  <li><a href="https://github.com/facebookresearch/llama">LLaMA</a></li>
</ol>

<ol>
  <li><a href="https://github.com/tatsu-lab/stanford_alpaca">Stanford Alpaca: An Instruction-following LLaMA Model</a></li>
</ol>

<ol>
  <li><a href="https://beebom.com/how-run-chatgpt-like-language-model-pc-offline/">How to Run a ChatGPT-Like LLM on Your PC Offline</a></li>
</ol>

<ol>
  <li><a href="https://www.smartspate.com/how-to-set-up-your-own-ai-alternative-to-chat-gpt-but-with-alpaca-on-your-vps-server/?utm_source=rss&utm_medium=rss&utm_campaign=how-to-set-up-your-own-ai-alternative-to-chat-gpt-but-with-alpaca-on-your-vps-server">How To Set Up Your Own AI Alternative to Chat-GPT But With Alpaca On Your VPS Server!</a></li>
</ol>

<hr class="with-margin">

![go]({{ site.baseurl }}/assets/img/2023-04-09/logo2.png){: .autofit-image}
<br>