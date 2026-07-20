---
layout: default
title: Monoids
---

Define the function $f : S \times S \rightarrow S$ as the binary operation on a set $S$, where $S \times S$ has all pairs $(x,y)$ when $x, y \in S$. The ordered pair, $(S, \circ)$ is a mnonoid if-

 - S is a set
 - $\circ$ is a binary operation on S, i.e. $\circ \ \ : \ \ S \times S \rightarrow S$
 - $(\forall x,y \in S)$ $a,b \in S \implies a \circ b \in S$ (Closure)
 - $(\forall x,y,z \in S)$ $(a \circ b) \circ c = a \circ (b \circ c)$ (Associativity)
 - $\exists e \in S$ such that $(\forall a \in S) \ \ e \circ a = a \circ e = a$

The element $e$ is known as the multiplicative identity, some structures do not possess such element, which are known as semigroups.

The identity element is unique, as if we hypothesize a new identity element, $e^'$, we have, $e = e \circ e^' = e' \circ e = e^'$.

For convenience we can write $a \circ b = ab$. For associativity, we can stretch it to three elements, $(a \circ b) \circ c = a \circ (b \circ c) = a \circ b \circ c = abc$.

Associativity holds for $n$ elements, which we will prove by induction-

First we define the left-associated product $P(a_{1}, ..., a_{n})$ as follows-
for $n = 1$, $P(a_1) = a_1$
for $n = 2$, $P(a_1, a_2) = a_1 a_2$
For $n > 2$, $P(a_{1}, ..., a_{n}) = P(a_{1}, ..., a_{n-1}) a_n$

Now, we have for $n = 1,2,3$ associativity holds. Now let for any $k < n$ (where $n \geq 4$) any arbitrary parenthesized product evaluates to the standard left-associated product.

Now take any arbitrary parenthesization of $n$ elements. Any full parenthesization splits the sequence to some binary operation, so the product can be written as-
$$X = (a_{1} \circ a_{2} ... a_k) \circ (a_{k+1} ... a_n)$$
as by our inductive hypothesis, $a_{1} \circ a_{2} ... a_k$ follows associativity, and the rest is arbitrarily multiplied. Now, we have $a_{1} \circ a_{2} ... a_k = P ($a_{1} \circ a_{2} ... a_k)$
