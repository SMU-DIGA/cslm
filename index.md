---
layout: default
title: Home
---


# Computer Science of Language Models

Let's build the computer science of language models together. 

---

## (Multimodal) Language Models as New Universal Computers

Language model is becoming the new universal computer, which can solve
even more problems than traditional computers. However, there is still
lacking the computer science of language models. 

What define the computer science? What make the computer science be the science? 
The computation complexity theory is one of the main reasons. So our question is:
Can we build the complexity theory (maybe empirically) for langauge models?


The traditional computer science is based on **the solving-verifying dichotomy**. 
Specifically, researchers build the computer science by checking the differences between
solving a problem and verifying a solution of the problem. For P problems, we can solve the 
problems and verifying the solutions of the problems in polynomial time. For NP problems, 
we can verify the solutions of the problems in polynomial time, but not necessarily solve the problems in 
polynomial time. 

As far as we can see, the differences of computer science of language models include:
1. **Generation-solving-verifying triad**, rather than the solving-verifying dichotomy. Traditional computers can only do solving and verifying, but LMs can also generate the problems. It is so difficult for traditional computers to generate the problems and investigate the complexity of generating the problems. But for LMs, we surely can do this. 
2. **Token as the basic operation**. The basic operation for traditional computers are computation operation, while for LMs, the basic operation is token. 
3. **Buggy**. With many-year efforts, we do not suffer in the system errors of traditional computers for solving and verifying, once programed correctly. However, LMs can hallucinate, i.e., make mistakes. We can not make sure that LMs always return the correct solutions even so-called correctly prompted. In this case, how to investigate this? 
4. **Multimodal**. Most traditional computers can only handle text and numerical. But multimodal LMs can handle audio, image/video and any modal of data. We can really build a universal theoretical understanding. 


This would be a new direction for us to understand the intrinsic properties of problems and multimodal LMs. 
Providing a universal perspective for us to design benchmarks, collect data, build model architectures and train the models.

**Welcome to THE new computer science!**

---

## Our Work

### 1. [Nondeterministic Polynomial-time Problem Challenge: An Ever-Scaling Reasoning Benchmark for LLMs](https://arxiv.org/abs/2504.11239) (April 2025)

Given that almost all benchmarks will be crushed in short time, i.e., higher than 90% accuracy within 1 year, and hacked, i.e., overfit to the current benchmarks. 
In this work, we propose the **ever-scalingness**, where we believe that a good benchmark should be scaling over complexity, i.e., the difficulty of generated problems can be increased continuously, 
instances, i.e., generating infinite instances to avoid overfitting, oversight, i.e., easy for verification even for very difficult problems, and coverage, i.e., be real-world relevant. 
These four desiderata should be the golden criteria for a good benchmark. 

Motivating by this, we propose NPPC, the first ever-scaling benchmark for LLMs. 

### 2. Language Models as Computers: A Computational Complexity Perspective

Ongoing and coming soon. 


---

## Existing Other Related Work

### Perspective: Shifting from Models to Problems

1. [The Second Half](https://ysymyth.github.io/The-Second-Half/)
2. [Welcome to the Era of Experience](https://storage.googleapis.com/deepmind-media/Era-of-Experience%20/The%20Era%20of%20Experience%20Paper.pdf)

### Theory

1. [Physics of Language Models](https://physics.allen-zhu.com/)
2. [Chain of Thought Empowers Transformers to Solve Inherently Serial Problems](https://arxiv.org/abs/2402.12875)
3. [Autoregressive Large Language Models are Computationally Universal](https://arxiv.org/abs/2410.03170)

### Benchmarking

1. [NPHardEval: Dynamic Benchmark on Reasoning Ability of Large Language Models via Complexity Classes](https://arxiv.org/abs/2312.14890)
2. [ZebraLogic: On the Scaling Limits of LLMs for Logical Reasoning](https://arxiv.org/abs/2502.01100)
3. [REASONING GYM: Reasoning Environments for Reinforcement Learning with Verifiable Rewards](https://arxiv.org/abs/2505.24760)

### Training

1. [SATURN: SAT-based Reinforcement Learning to Unleash Language Model Reasoning](https://arxiv.org/abs/2505.16368)
2. [NP-Engine: Empowering Optimization Reasoning in Large Language Models with Verifiable Synthetic NP Problems](https://www.arxiv.org/abs/2510.16476)
3. [RLVE: Scaling Up Reinforcement Learning for Language Models with Adaptive Verifiable Environments](https://arxiv.org/abs/2511.07317)

### Memory

1. [How much do language models memorize?](https://arxiv.org/abs/2505.24832)
2. [The Landscape of Memorization in LLMs: Mechanisms, Measurement, and Mitigation](https://arxiv.org/abs/2507.05578)
3. [Information Capacity: Evaluating the Efficiency of Large Language Models via Text Compression](https://arxiv.org/abs/2511.08066)
4. [Retaining by Doing: The Role of On-Policy Data in Mitigating Forgetting](https://arxiv.org/abs/2510.18874)