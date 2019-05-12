---
permalink: introduction
title: Introduction
layout: default
---

# {{page.title}}

Reinforcement learning has become extremely popular lately. Advances in techniques and distributed processing has allowed reinforcement learning agents to [beat the world champion at Go](https://deepmind.com/research/alphago/) and [play competitively against world leaders at Dota 2](https://openai.com/five/).

In this series, we build up a deep theoretical understanding of reinforcement learning by combining theory and implementations. We will be using the [Python](https://www.python.org/) programming language, along with an assortment of libraries such as [numpy](https://www.numpy.org), [tensorflow](https://www.tensorflow.org/), and [gym](https://gym.openai.com/). We assume the reader has familiarity with programming in Python. We will also be making extensive use of [jupyter notebooks](https://jupyter.org/).

### The Basic Reinforcement Learning Loop

There are two main entities in reinforcement learning: the **agent** and the **environment**.

{: style="text-align:center"}
![rl-loop]({{site.url}}/assets/images/rl.png)

The agent is responsible for choosing **actions** \\( a_t \\) based on the current **state** \\( s_t \\). In turn, the environment changes according the action that the agent took. The environment then provides the agent with the next state \\( s_{t+1} \\), and also a **reward** \\( r_t \\) that represents how good or bad it was to choose that action in that state.

The driving idea behind reinforcement learning is the **reward hypothesis**:

> Every action of a rational agent can be thought of as seeking to maximize some cumulative scalar reward signal.

Our goal is for the agent to learn a **policy**, a set of rules for choosing actions based on the current state, that maximizes the cumulative rewards.

Over the course of several lessons, we will build up an understanding of two main classes of policies: [**\\( Q \\) -learning**]({{site.url}}/q-learning) and [**policy gradients**]({{site.url}}/policy-gradients).
