---
layout: default
title: Home
---

<style>
h1 {
    text-align: center;
}
</style>


# Computer Science of Language Models

Welcome to the era of new computer science! 

Let's be the new Cook and find the "NPC" problems for language models!

---

## (Multimodal) Language Models as New Universal Computers

<div align="center">
<img src="{{ site.baseurl }}/assets/cslm.svg"  style="width:50%">
</div>

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
1. **Generating-solving-verifying triad**, rather than the solving-verifying dichotomy. Traditional computers can only do solving and verifying, but LMs can also generate the problems. It is so difficult for traditional computers to generate the problems and investigate the complexity of generating the problems. But for LMs, we surely can do this. 
2. **Token as the basic operation**. The basic operation for traditional computers are computation operation, while for LMs, the basic operation is token. 
3. **Buggy**. With many-year efforts, we do not suffer in the system errors of traditional computers for solving and verifying, once programed correctly. However, LMs can hallucinate, i.e., make mistakes. We can not make sure that LMs always return the correct solutions even so-called correctly prompted. In this case, how to investigate this? 
4. **Multimodal**. Most traditional computers can only handle text and numerical, they can handle the images in pixel level but cannot understand them from pixel to concept, therefore, they fail to operate the images like human. But multimodal LMs can handle audio, image/video and any modal of data. We can really build a universal theoretical understanding.
5. **Generalizability**. Algorithms, the core of traditional computer science, are usually problem-specific. While (multimodal) LMs are general-purpose. Evaluating the models on different problems can reveal the fundamental properties of models, and letting different models to solve one problems will reveal the fundamental properties of the problems. 
From LSTM, to transformer, to diffusion LMs, this is the same to build more advanced computers; from QA, to generation, to math, to HLE, to SWE-bench, this is the same to find the NPC/NP-hard problems.


This would be a new direction for us to understand the intrinsic properties of problems and multimodal LMs. 
Providing a universal perspective for us to design benchmarks, collect data, build model architectures and train the models.
The ultimate goal of computer science of language models is **completing the tasks correctly with less tokens (maybe also less runtime and memory)**.


| Aspect | Traditional Computer Science | Computer Science of Language Models |
|--------|------------------------------|--------------------------------------|
| **Problem-Solving Paradigm** | Solving-verifying dichotomy | Generating-solving-verifying triad |
| **Basic Operation** | Computation operations | Token operations |
| **Reliability** | Deterministic (correct if programmed correctly) | Non-deterministic (can hallucinate/make mistakes) |
| **Modality** | Text and numerical only; pixel-level image processing without conceptual understanding | Multimodal (audio, image, video, text) with conceptual understanding |
| **Complexity Analysis** | Focus on time/space complexity for solving and verifying | Include complexity of generation; token efficiency |
| **Ultimate Goal** | Completing tasks with less time and memory | Completing tasks correctly with less tokens (and potentially less runtime/memory) |
| **Research Focus** | Algorithm correctness and efficiency | Intrinsic properties of problems, benchmark design, data collection, model architecture, and training |


[//]: # (**Welcome to the era of new computer science!**)


---

## Our Work

### 1. [Nondeterministic Polynomial-time Problem Challenge: An Ever-Scaling Reasoning Benchmark for LLMs](https://arxiv.org/abs/2504.11239) (April 2025)

Given that almost all benchmarks will be crushed in short time, i.e., higher than 90% accuracy within 1 year, and hacked, i.e., overfit to the current benchmarks. 
In this work, we propose the **ever-scalingness**, where we believe that a good benchmark should be scaling over complexity, i.e., the difficulty of generated problems can be increased continuously, 
instances, i.e., generating infinite instances to avoid overfitting, oversight, i.e., easy for verification even for very difficult problems, and coverage, i.e., be real-world relevant. 
These four desiderata should be the golden criteria for a good benchmark. 

Motivating by this, we propose NPPC, the first ever-scaling benchmark for LLMs. 

<div align="center">
<img src="{{ site.baseurl }}/assets/nppc.svg"  style="width:80%">
</div>

### 2. Language Models as Computers

Ongoing and coming soon. 


---

## Existing Other Related Work

### Perspective: Shifting the Focus from Models to Problems

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


### Empirical Laws

1. [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361)
2. [Training Compute-Optimal Large Language Models](https://arxiv.org/abs/2203.15556)


### Training

1. [SATURN: SAT-based Reinforcement Learning to Unleash Language Model Reasoning](https://arxiv.org/abs/2505.16368)
2. [NP-Engine: Empowering Optimization Reasoning in Large Language Models with Verifiable Synthetic NP Problems](https://www.arxiv.org/abs/2510.16476)
3. [RLVE: Scaling Up Reinforcement Learning for Language Models with Adaptive Verifiable Environments](https://arxiv.org/abs/2511.07317)

### Memory


#### Internal Memory

1. [How much do language models memorize?](https://arxiv.org/abs/2505.24832)
2. [The Landscape of Memorization in LLMs: Mechanisms, Measurement, and Mitigation](https://arxiv.org/abs/2507.05578)
3. [Information Capacity: Evaluating the Efficiency of Large Language Models via Text Compression](https://arxiv.org/abs/2511.08066)
4. [Retaining by Doing: The Role of On-Policy Data in Mitigating Forgetting](https://arxiv.org/abs/2510.18874)

#### External Memory

The mechanism of the external memory is still not very clear. RAG and database can be viewed as the external memory. 
That still depends on LM's capabilities to process the contents. It would be an agentic system. 

1. [Unveil the Duality of Retrieval-Augmented Generation: Theoretical Analysis and Practical Solution](https://openreview.net/forum?id=jaoYoivyjD)


### Tools

How to theoretically deal with the tool using/creation in LMs. One view is that tool using can make LMs more token-efficient and less erroneous. All agentic operations, including
retrieval, searching, tool calling, tool creation, can be counted into tokens. 

1. [Understanding Tool-Integrated Reasoning](https://arxiv.org/abs/2508.19201)


