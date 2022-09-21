---
title: "Current Research Directions"
permalink: /research/
author_profile: true
---
* [Music Difficulty Detection](#fine-grained-music-difficulty-analysis)
* [Set-Based Prediction for Open Vocabulary Models](#hierarchical-set-based-prediction-for-open-vocabulary-models)
* [Implicit Regularization in SGD](#implicit-and-explicit-regularization-in-sgd-for-deep-networks)


# Past Research Projects
* [Social Media Addiction](#social-media-addiction)
* [Extremism](#online-extremism-and-hate-speech)

<br/><br/>

# Fine-Grained Music Difficulty Analysis and Mistake Prediction
<img src="/staircase.png"
     alt="staircase"
     style="float: left; margin-right: 10px;"
     height=550px
     width=750px/>
<figcaption align = "center"><b>Figure from <a href="https://www.researchgate.net/publication/260426079_An_experimental_validation_of_Temporal_Semiotic_Units_and_Parameterized_Time_Motifs" target="_blank">this</a> paper</b></figcaption>

Recent developments within the Music Information Retrieval (MIR) space have seen large advances in the ability to generate and analyze music. While much of the focus within MIR has been on music generation and analysis tools that inform industry use cases (e.g. music recommendation, genre classification), comparably little attention has been given to more pedagogical use cases, especially with regards to **assessing music difficulty at a fine-grained level (e.g. bar-by-bar) level**.

Here, we have been investigating how we can leverage user performance data to model musical difficulty and forecast incorrect passages within performance without ever seeing the ground truth musical representation.

# Hierarchical Set-Based Prediction for Open Vocabulary Models
<img src="/dogs.webp"
     alt="dog breeds"
     style="float: left; margin-right: 10px;"
     height=550px
     width=750px/>

Open vocabulary models, especially CLIP, have seen large successes in Zero-shot image classification by embedding the downstream set of classes into textual "prompts" and generating a set of similarity scores between any image and the given class prompts. While existing work on improving CLIP has focused on finetuning CLIP on downstream tasks or improving the quality of the given prompts, we instead have investigated a parallel line of work by framing the class prediction task as a classification problem over **subclasses** of each original superclass. Here, we can leverage CLIP's ability to distinguish between fine-grained concepts (e.g. huskies v.s. corgis) and then use the class-to-subclass mapping to return our predictions into the original superclass space. 


# Implicit and Explicit Regularization in SGD for Deep Networks
<img src="/reg.png"
     alt="sgd resnet"
     style="float: left; margin-right: 10px;"
     height=550px
     width=750px/>


One of the many open questions with regards to Deep Learning (DL) concerns the fact that in large, overparametrized networks, models trained with mini-batch Stochastic Gradient Descent (SGD) display improved generalization performance over full-batch methods. While much research has focused on analyzing SGD through the lens of additive or multiplicative noise, we instead have focused on the theories hat attribute SGD's generalization performance to the implicit regularization of certain quantities.

In this project, I have conducted a large-scale empirical study of different explicit regularization mechanisms (like the one pictured above) across a wide range of model types and image recognition benchmarks, and additionally have investigated other open questions within the field of implicit regularization, such as the dependence on the batch size used to calculate the regularization terms.

<br/>

# Social Media Addiction
<img src="/sma.jpeg"
     alt="stock sma photo"
     style="float: left; margin-right: 10px;"
     height=550px
     width=750px/>


Generally, when everyday people talk about being "addicted to social media", a particular kind of image is often evoked: some young person, wasting away their time, endlessly scrolling through whatever social network is their favorite. I take issue with this common normative argument, since it is rather divorced from actual scientific properties of addiction (e.g. adjustment to baselines, undue damage to one's life, withdrawal mechanics) and seems to rest on the notion that "social media is bad, and therefore, using it a lot must be *extra* bad." Instead, I have been researching how individual users get addicted to **online interaction and engagement**, focusing chiefly on Twitter.

In order to model how an individual user responds to trends in their percieved engagement on Twitter, I have been investigating Bayesian autoregressive modeling (via Stan), where user post frequency is assumed to be drawn from a Negative Binomial distribution. Such modeling assumptions have the benefit over traditional count-data analyses (e.g. Poisson regression) by directly modeling overdispersion in the data, thus account for the often high variability in post frequency that user data exhibits.

<br/>

# Online Extremism and Hate Speech
<img src="/xtm.png"
     alt="Ideological Network on The Red Pill subreddit"
     style="float: left; margin-right: 10px;"
     height=550px
     width=750px/>
<figcaption align = "center"><b>Figure from <a href="https://arxiv.org/abs/2110.00626" target="_blank">this</a> great paper</b></figcaption>

There is currently a growing body of research within the applied machine learning community that seeks to quantify and track extremist behavior and hate speech online. I have been particularly interested in thinking about the evolution of **extremist communities and forums** (e.g. The Red Pill on Reddit, /pol/ on 4chan, etc.), as these less mainstream websites are often the progenitors of hateful rhetoric and are trafficked by possible domestic terrorists.

Recently, I have been investigating how the ideological network of a given website (pictured above is The Red Pill, for instance) is structured and how such structure evolves across time scales. This generally involves generating a topic model of the underlying text corpus, and building the linkage network given these probabilities for different timescales.

At a high level, this per-website analysis affords us the ability to measure the implications of certain administrative choices (e.g. making posts anonymous or self-delete after a fixed amount of time) on the formation and interconnectedness of different fringe viewpoints.