# Computer Science for Language Models

Let's build the computer science for language models together. 

---

## (Multimodal) Language Models as New Universal Computers

Language model is becoming the new universal computer, which can solve
even more problems than traditional computers. However, there is still
lacking the computer science for language models. 

What define the computer science? What make the computer science be the science? 
The computation complexity theory is one of the main reasons. So our question is:
Can we build the complexity theory (maybe empirically) for langauge models?


The traditional computer science is based on **the solving-verifying dichotomy**. 
Specifically, researchers build the computer science by checking the differences between
solving a problem and verifying a solution of the problem. For P problems, we can solve the 
problems and verifying the solutions of the problems in polynomial time. For NP problems, 
we can verify the solutions of the problems in polynomial time, but not necessarily solve the problems in 
polynomial time. 

As far as we can see, the differences of computer science for language models include:
1. Generation-solving-verifying triad, rather than the solving-verifying dichotomy. Traditional computers can only do solving and verifying, but LMs can also generate the problems. It is so difficult for traditional computers to generate the problems and investigate the complexity of generating the problems. But for LMs, we surely can do this. 
2. Token as the basic operation. The basic operation for traditional computers are computation operation, while for LMs, the basic operation is token. 
3. Buggy. With many-year efforts, we do not suffer in the system errors of traditional computers for solving and verifying, once programed correctly. However, LMs can hallucinate, i.e., make mistakes. We can not make sure that LMs always return the correct solutions even so-called correctly prompted. In this case, how to investigate this? 
4. Multimodal. Most traditional computers can only handle text and numerical. But multimodal LMs can handle audio, image/video and any modal of data. We can really build a universal theoretical understanding. 

5. This can bring lots of different investigations.

---

## Existing Work

### Theory

1. [Physics of Language Models](https://physics.allen-zhu.com/)

### Benchmarking

1. [NPHardEval: Dynamic Benchmark on Reasoning Ability of Large Language Models via Complexity Classes](https://arxiv.org/abs/2312.14890)
2. [ZebraLogic: On the Scaling Limits of LLMs for Logical Reasoning](https://arxiv.org/abs/2502.01100)
3. [Nondeterministic Polynomial-time Problem Challenge: An Ever-Scaling Reasoning Benchmark for LLMs](https://arxiv.org/abs/2504.11239)

### Training

1. [SATURN: SAT-based Reinforcement Learning to Unleash Language Model Reasoning](https://arxiv.org/abs/2505.16368)
2. [NP-Engine: Empowering Optimization Reasoning in Large Language Models with Verifiable Synthetic NP Problems](https://www.arxiv.org/abs/2510.16476)
3. [RLVE: Scaling Up Reinforcement Learning for Language Models with Adaptive Verifiable Environments](https://arxiv.org/abs/2511.07317)


### Memory

1. [How much do language models memorize?](https://arxiv.org/abs/2505.24832)
2. [The Landscape of Memorization in LLMs: Mechanisms, Measurement, and Mitigation](https://arxiv.org/abs/2507.05578)