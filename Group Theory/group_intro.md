---
layout: default
title: Group Theory- Introduction
---

A group is a structure extensively studied in abstract algebra for it's versatility to explain symmetries etc. We first explain the notion of binary operations-

A binary operation $\circ$ on a set A is defined as a function $\circ : A \times A \rightarrow A$ (closed under operation). The binary operation is associative, i.e. $(\forall a,b,c \in A) \ \ a \circ (b \circ c) = (a \circ b) \circ c$. If the relation $(\forall a,b \in A) \ \ a \circ b = b \circ a$ hold, the binary relation is called commutative or abelian.

For a set $A$ and a binary relation $\circ$, a group is an ordered pair $(G, \circ)$ satisfying the following axioms-

i) $\exists e \in G$ such that $(\forall a \in G) \ \ e \circ a = a \circ e = a$. The element $e$ is known as the identity, and written as $1$ or $0$ when the binary operation is multiplication and addition, respectively.
ii) $\forall a \in G \exists a^{-1}$ such that $a \circ a^{-1} = a^{-1} \circ a = e$

Also, a group is closed under addition and associative under the binary operation defined on it, but it is inherited from the definitions of binary relations.

The smallest group or the trivial group is $\{e\}$, so groups are nonempty.

We write $x \circ x = x^2$ for convenience and $x^n$ is similarly defined.

If we want to create a group with an element $x$, we get the group $<x> = \{e, x, x^-1, x^2, x^-2, x^3, x^-3, .....,\}$. The elements keep appearing for the group axioms, multiplication is closed under addition so $x \in G \implies x \circ x \in G$, and similarly $x^3,.. x^n$ is in $G$. Also the inverses get included. Such groups are known as cyclic groups. Relations, generators and presentations will be discussed later properly.
