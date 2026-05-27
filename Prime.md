<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# My Mathematics Portfolio

Welcome to my transition from engineering to pure math. Here is a collection of proofs I am digitizing.

## Theorem 1: Infinitude of Primes
**Theorem:** There are infinitely many primes.

**Proof:** Assume for contradiction that there is a finite number of primes, say $p_1, p_2, \dots, p_n$. 
Consider the number:

$$P = \left(\prod_{i=1}^{n} p_i\right) + 1$$

Either $P$ is prime or it is composite:
1. If $P$ is prime, then $P$ is a new prime not in our list, a contradiction.
2. If $P$ is composite, it must be divisible by some prime $p$. However, if $p$ is one of the primes on our list, it must divide the product $\prod_{i=1}^{n} p_i$. 

Therefore, $p$ must divide the difference:

$$P - \prod_{i=1}^{n} p_i = 1$$

Since no prime can divide $1$, we reach a contradiction. Hence, there are infinitely many primes. $\blacksquare$

