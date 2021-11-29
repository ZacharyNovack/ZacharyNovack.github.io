---
title: "Current Research Directions"
permalink: /research/
author_profile: true
---
## Social Media Addiction
<img src="/sma.jpeg"
     alt="stock sma photo"
     style="float: left; margin-right: 10px;"
     height=500px
     width=700px/>

Generally, when everyday people talk about being "addicted to social media", a particular kind of image is often evoked: some young person, wasting away their time, endlessly scrolling through whatever social network is their favorite. I take issue with this common normative argument, since it is rather divorced from actual scientific properties of addiction (e.g. adjustment to baselines, undue damage to one's life, withdrawal mechanics) and seems to rest on the notion that "social media is bad, and therefore, using it a lot must be *extra* bad." Instead, I have been researching how individual users get addicted to **online interaction and engagement**, focusing chiefly on Twitter.

In order to model how an individual user responds to trends in their percieved engagement on Twitter, I have been investigating Bayesian autoregressive modeling (via Stan), where user post frequency is assumed to be drawn from a Negative Binomial distribution. Such modeling assumptions have the benefit over traditional count-data analyses (e.g. Poisson regression) by directly modeling overdispersion in the data, thus account for the often high variability in post frequency that user data exhibits.


## Online Extremism and Hate Speech
<img src="/xtm.png"
     alt="Ideological Network on The Red Pill subreddit"
     style="float: left; margin-right: 10px;"
     height=500px
     width=700px/>


There is currently a growing body of research within the applied machine learning community that seeks to quantify and track extremist behavior and hate speech online. I have been particularly interested in thinking about the evolution of **extremist communities and forums** (e.g. The Red Pill on Reddit, /pol/ on 4chan, etc.), as these less mainstream websites are often the progenitors of hateful rhetoric and are trafficked by possible domestic terrorists.

Recently, I have been investigating how the ideological network of a given website (pictured above is The Red Pill, for instance) is structured and how such structure evolves across time scales. This generally involves generating a topic model of the underlying text corpus, and building the linkage network given these probabilities for different timescales.

At a high level, this per-website analysis affords us the ability to measure the implications of certain administrative choices (e.g. making posts anonymous or self-delete after a fixed amount of time) on the formation and interconnectedness of different fringe viewpoints.