---
layout: post
title: [Paper Review] Attention Is All You Need
tags: [paper, attention, transformers,nlp, sequence modeling, rnn, lstm, gru]
---

ln this posting, I will very briefly review the paper Attention Is All You Need. I first want to summarize the whole paper by answering the following questions. Those questions are adopted from Andrew Ng’s career advice. You can see it [here](https://scottsuk0306.github.io/2022/07/04/how-to-read-papers.html), too.

If you want rigorous mathematical details about the transformer architecture and multi-head attention, I recommend you to move onto the original paper after reading this post.

## What did authors try to accomplish?
  
  For sequence modeling and transduction problems, recurrent neural networks were widely used and have been state-of-the-art approach for an amount of time. However, it works as sequentially and the constraint of sequential computation has not been resolved for a long time.
  
  The authors proposed the Transformer, eschewing recurrence and depend entirely on attention mechanism. It allows significantly more parallelization and can reach a new state of the art in translation quality.

## What were the key elements of the approach?
  
  I think the model architecture of Transformer is the key element of the approach. Focusing at how authors dealt with sequential modeling without sequential computation is anohter important aspect of the whole paper.

## What can you use yourself?
  
  I’m interested in solving general NLP problems. Currently, I’m into question answering and information retrieval. I briefly know that current NLP research trends are highly dependent on transformers, but only in NLP but also Vision, Graphs, and so much more. I would like to use Transformers, or Transformer-based models for my side project.

## What other references do you want to follow?
  
  1. After realizing the great amount of potential inside transformers, I became really curious about the impact of Transformers and the research trends throughout the whole field. To resolve my curiousity, I’m planning to read some survey papers on transformers.
     - [Survey of Transformers](https://arxiv.org/abs/2106.04554)
     - [Visualizing Transformers for NLP: A Brief Survey](https://ieeexplore.ieee.org/abstract/document/9373074)
     - [Efficient Transformers: A Survey](https://dl.acm.org/doi/abs/10.1145/3530811)
     - [Transformers in Vision: A Survey](https://dl.acm.org/doi/abs/10.1145/3505244)
  
  2. Transformer-based language models
     - [GPT-1](https://www.cs.ubc.ca/~amuham01/LING530/papers/radford2018improving.pdf)
     - [GPT-2](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
     - [BERT](https://arxiv.org/abs/1810.04805)
  
  3. Supplementary materials
     - [Youtube video on text-to-text transformers](https://www.youtube.com/watch?v=v7diENO2mEA&t=1215s)
     - [The Annotated Transformer](https://nlp.seas.harvard.edu/2018/04/03/attention.html)
     - [Formal Algorithms for Transformers](https://arxiv.org/abs/2207.09238)


  ### Vocabularies
  Those are vocabularies that I did not get while reading the paper. I organized the meanings here.
  1. albeit: despite the stated thing; although
  2. transduction, transduction model: Transduction is reasoning from observed, specific (training) cases to specific (test) cases. In contrast, induction is reasoning from observed training cases to general rules, which are then applied to the test cases. ([Reference](https://towardsdatascience.com/inductive-vs-transductive-learning-e608e786f7d))

  ### Questions
  Those are questions I had while reading the paper. I will continuosly try to answer them on my own, and I wrote them here for archiving purposes.

  1. Is convolution sequential? (or has similar computational complexity to sequential operations?)
  2. Why is residual connection used?
  3. Why is layer normalization used?
