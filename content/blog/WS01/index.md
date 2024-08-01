+++
authors = ["Matteo Risso"]
title = "My first post"
description = "Weekly Summary 01."
date = 2024-12-01
[taxonomies]
tags = ["Weekly Summary"]
[extra]
banner = "ws01.jpg#pixels"
toc = true
+++

# Disclaimer
This is my first post tagged as **Weekly Summary**. 
Honestly, I started this "project" mainly because I would like to follow the "learning in public" philosophy.
Writing down every day something is definitely to much for someone like me who doesn't like to write, but I think that a weekly summary is a good compromise.
By the way, this is public but I don't know if someone will ever read this. Anyway, I don't care.

Every section will deal with something that I read, studied or worked on during the week.

Here it is a picture of my cat, because, why not!

<figure>

![ef](ef.jpg)
<figcaption>Elio Fabrizio, the cat of mine and my girlfriend.</figcaption>
</figure>

# Backpropagation Algorithm
As a Deep Learning practitioner for about 3 years, I should say **yes**, I know really well how to compute derivatives and how to apply the backpropagation algorithm.
Honestly, PyTorch is such a niece piece of code, that yes, I know how stuff works in principle, but last time I computed a derivative by hand was probably during Calculus.
Shame on me, I know.

For a research project that I'm working on, I need to deep dive into this so I started to read some nice resources about the topic.

I will briefly list them here.

#### [Derivatives, Backpropagation, and Vectorization](https://cs231n.stanford.edu/handouts/derivatives.pdf)
*by Justin Johnson, Stanford University.*

This is are really nice LaTex notes that first explain derivatives starting from the scalar case, moving to the vector case, then to the matrix case, and last tensors (i.e., the case of DNNs).

Finally, a real example is given where it is shown the backpropagation algorithm applied to a linear layer. A really nice passage is how we can avoid to compute the full (generalized) Jacobian matrix. Such matrix even for a small network can be huge and computationally expensive to compute.

#### [Backpropagation for a Linear Layer](https://cs231n.stanford.edu/handouts/linear-backprop.pdf)
*by Justin Johnson, Stanford University.*

Same author, same topic, but this time the focus is on the backpropagation algorithm applied to a little bit more complex linear layer.

#### [Backward Pass for a Convolutional Layer](https://sites.cc.gatech.edu/classes/AY2021/cs7643_spring/assets/L11_CNNs.pdf)
*by Unknown Author, Georgia Tech.*

These are slides from a course at Georgia Tech. The focus is on the backward pass of a convolutional layer.
Honestly, I'm definetely more a LaTex notes person than a slide person, but the content is good enough.
It is basically the same content of the previous notes, but applied to a convolutional layer.

# [KID-PPG](https://arxiv.org/abs/2405.09559)
*by Christodoulos Kechris, Jonathan Dan, Jose Miranda, David Atienza, EPFL*

A really nice paper about PPG-based Heart Rate Estimation using a Knowledge-Informed Deep Learning Model.
They achieve SotA results on the [PPG-DaLiA](https://archive.ics.uci.edu/dataset/495/ppg+dalia) dataset.
> PPG-DaLiA is a publicly available dataset for PPG-based heart rate estimation. This multimodal dataset features physiological and motion data, recorded from both a wrist- and a chest-worn device, of 15 subjects while performing a wide range of activities under close to real-life conditions. The included ECG data provides heart rate ground truth. The included PPG- and 3D-accelerometer data can be used for heart rate estimation, while compensating for motion artefacts.

During my master thesis, I worked exactly on this topic and we were the SotA on this dataset. Damn, you beat me!
Anyway, I'm really happy to see that the research is going on and that new models are proposed.

What I really enjoied about this paper is this sentence:
> **Although deep learning methods trained as a data-driven inference problem offer promising solutions, they often underutilize ex- isting knowledge from the medical and signal processing community.**

This is exactly what I think. We should not forget the past and the knowledge that we have.
Deep Learning is cool, but we shall not reduce to dumb monkeys (I love monkeys, I swear) that limits to throw some data to a soup of linear algebra.

{% alert(caution=true) %}
Curios thing: I'm writing this stuff in vscode with copilot enabled. It stopped working when I said stuff above. Probably it doesn't like monkeys.
{% end %}

# Readings
- I started reading, with my girlfriend, the book *Gödel, Escher, Bach: an Eternal Golden Braid* by Douglas Hofstadter. Right now I don't have any opinions, but it is really **huge**. I hope to finish it.
- I read the [‘Sensational breakthrough’ marks step toward revealing hidden structure of prime numbers](https://www.science.org/content/article/sensational-breakthrough-marks-step-toward-revealing-hidden-structure-prime-numbers) article about the recent breakthrough in the field of Riemann Hypothesis. I'm not a mathematician (at least not yet), but I'm really fascinated by this kind of stuff.
-  I read some other stuff from Hacker News, but I don't remember what. I should start to take notes.

# Random Ideas
Few weeks ago I discovered a really interesting twitter account (I'll never say x, sorry Elon) of a crazy brazilian guy known as [Victor Taelin](https://x.com/VictorTaelin).
He founded a company called HOC which wants to unlock the full potential of parallel computing by proposing a new (well, really old) paradigm known as *Interaction Calculus*.
You can read more in this really nice [gist](https://gist.github.com/VictorTaelin/77fd5a2a8a4a07e1da6157ebca3c7cf1).

This guy is an expert about functional languages, type theory and proof checkers. I started reading something thanks to him and I'm really fascinated by this stuff.

Today (01/08/2024) I randomly found this [repo](https://github.com/sickcodes/Docker-OSX) about running macOS in a docker container using QEMU. And I'm wondering what if we can emulate platforms using QEMU on GPUs with **Interaction Calculus**? Honestly this idea is not mine and comes from a comment in a blog in the HOC discord server. It such a cool idea!
Btw, [Getting started with qemu](https://drewdevault.com/2018/09/10/Getting-started-with-qemu.html). Read in case of fire.

Speaking of nice *functional* bros on twitter (not X, sorry Elon) there is also this guy [Dmitrii Kovanikov](https://x.com/ChShersh). He is an OCAML chad and he just started a blog post series about Category Theory for SWEs. I'm really excited to read it.
This is the first post -> [Pragmatic Category Theory | Part 1: Semigroup Intro](https://dev.to/chshersh/pragmatic-category-theory-part-1-semigroup-intro-1ign).