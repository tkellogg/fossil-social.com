---
title: "Open Source & Transparent"
layout: page
---

Fossil is [open source][oss] so that anyone can see and peer review the algorithm [on Github][gh]. You should be able
to verify our claim, that the algorithm is optimized for you. And if you think it could be optimized
better you can ask us to improve it, or even improve it yourself and send a pull request. That's
what open source is all about. Transparency.

## The Algorithm
The algorithm is fairly simple, at a high level:

1. Download posts
2. Group them together into clusters
3. Use AI to generate a label for the cluster

Step 2, the clustering part, used to be a lot harder prior to large language models (LLMs) in 2022-23.
LLMs let us understand text posts and compare how different two posts are. They act as a sort of
"radar", letting us see and understand the text before we actually read it.

Details:
* Clustering is done via [K-Means][kmeans], a traditional machine learning technique
* Text is converted to K-Means input via [embeddings][emb]. This leverages a lot of the abilities of a full LLM,
  but is just an intermediate representation that we can do math on (i.e. we feed it into K-Means).
* The produced clusters all share something in common, we use `gpt-3.5-turbo` (i.e. the ChatGPT model)
  to summarize the posts and come up with a label for the group.

We'll make updates in the future, but we'll always remain transparent about how it works.


## Do I need to pay?
No. The [fossil-social.com][site] is intended to be the fastest way to get started with Fossil. Originally,
we noticed that a lot of people weren't using fossil because it took too much time to setup the project.
We hope that $4/month is a low enough cost to not deter too many people. However, you can absolutely run
the project on your own laptop, that works fine too.


 [gh]: https://github.com/tkellogg/fossil/
 [oss]: https://timkellogg.me/blog/2023/12/19/fossil
 [mod]: https://timkellogg.me/blog/2024/01/17/htmx
 [site]: https://www.fossil-social.com/
 [kmeans]: https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html
 [emb]: https://simonwillison.net/2023/Oct/23/embeddings/
