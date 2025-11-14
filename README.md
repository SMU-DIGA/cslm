# Computer Science for Language Models

Let's build the computer science for language models. 

---

## LM as New Universal Computers

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

This can bring lots of different investigations.