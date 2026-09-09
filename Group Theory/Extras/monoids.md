---
layout: default
title: Monoids
---

Define the function $f : S \times S \rightarrow S$ as the binary operation on a set $S$, where $S \times S$ has all pairs $(x,y)$ when $x, y \in S$. The ordered pair, $(S, \cdot)$ is a mnonoid if-

 - S is a set
 - $\cdot$ is a binary operation on S, i.e. $\cdot: S \times S \rightarrow S$
 - $(\forall x,y \in S)$ $a,b \in S \implies a \cdot b \in S$ (Closure)
 - $(\forall x,y,z \in S)$ $(a \cdot b) \cdot c = a \cdot (b \cdot c)$ (Associativity)
 - $\exists e \in S$ such that $(\forall a \in S) \ \ e \cdot a = a \cdot e = a$

The element $e$ is known as the multiplicative identity, some structures do not possess such element, which are known as semigroups.

The identity element is unique, as if we hypothesize a new identity element, $e'$, we have, $e = e \cdot e' = e' \cdot e = e'$.

For convenience we can write $a \cdot b = ab$. For associativity, we can stretch it to three elements, $(a \cdot b) \cdot c = a \cdot (b \cdot c) = a \cdot b \cdot c = abc$.

Associativity holds for $n$ elements, which we will prove by induction-

Any fully parenthesized product of $n$ elements $a_1, a_2, \dots, a_n$ in a monoid $M$ yields the same result, which is equal to the standard product $\prod_{i=1}^n a_i$.

Let $P$ be any fully parenthesized product of $n$ elements $a_1, a_2, \dots, a_n$. We use strong induction on $n$.

Base Cases ($n = 1, 2$):
For $n = 1$, $P = a_1 = \prod_{i=1}^1 a_i$.
For $n = 2$, the only valid parenthesization is $(a_1 \cdot a_2) = \prod_{i=1}^2 a_i$.

Assume that for all $1 \le k < n$, every valid parenthesization of $k$ elements equals the standard product of those $k$ elements.

Now consider a fully parenthesized product $P$ of $n$ elements. By the definition of a binary operation, $P$ must be the product of two smaller parenthesized expressions:
$$P = P_1 \cdot P_2$$
where $P_1$ is a fully parenthesized product of the first $m$ elements ($a_1, \dots, a_m$) and $P_2$ is a fully parenthesized product of the remaining $n - m$ elements ($a_{m+1}, \dots, a_n$) for some $1 \le m < n$.

Since $m < n$ and $n - m < n$, we apply the strong inductive hypothesis to both $P_1$ and $P_2$:
$$P_1 = \prod_{i=1}^m a_i \quad \text{and} \quad P_2 = \prod_{j=m+1}^n a_j$$
Therefore, we have:
$$P = \left( \prod_{i=1}^m a_i \right) \cdot \left( \prod_{j=m+1}^n a_j \right)$$
By the Lemma, this expression simplifies to:
$$P = \prod_{k=1}^n a_k$$
