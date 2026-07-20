---
layout: default
title: Monoids
---

Define the function $f : S \times S \rightarrow S$ as the binary operation on a set $S$, where $S \times S$ has all pairs $(x,y)$ when $x, y \in S$. The ordered pair, $(S, \circ)$ is a mnonoid if-

 - S is a set
 - $\circ$ is a binary operation on S, i.e. $\circ \ \ : \ \ S \times S \rightarrow S$
 - $(\forall x,y \in S)$ $a,b \in S \implies a \circ b \in S$ (Closure)
 - $(\forall x,y,z \in S)$ $(a \circ b) \circ c = a \circ (b \circ c)$ (Associativity)
 - $exists e \in S$ such that $(\forall a \in S) \ \ e \circ a = a \circ e = a$
