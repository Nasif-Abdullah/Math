---
layout: default
title: Order Theory- Introduction
---

This is a rigorous definition to relations, we often encounter such relations like greater than, equals to etc. This branch of mathematics deal with comparing things, grouping things, and putting things in a specific sequence.                                                                            
## The building block- Relations
A binary relation on a set $$A$$ is a way of defining an universal connection within any two elements of a set. Formally, we define the relation $$R\:(aRb)$$ within two elements $$a,b\: \forall a,b \in A$$ when it follows the following properties-

- <b>Reflexive:</b> Every element is related to itself ($$aRa$$)
- <b>Symmetric:</b> If $$a$$ is related to $$b$$, then $$b$$ is related to $$a$$ ($$aRb \rightarrow bRa$$)
- <b>Antisymmetric:</b> $$aRb \wedge bRa \rightarrow a = b$$
- <b>Transitive:</b> $$aRb \wedge bRc \rightarrow aRc$$

## Equivalence Relations 

Can be explained as grouping, an equivalence relation clusters elements that "share a common trait". An equivalence relation, $$a \sim b$$, similarly, satisfies the following relations-

- <b>Reflexive:</b> $$a \sim a$$
- <b>Symmetric:</b> $$a \sim b \rightarrow b \sim a$$
- <b>Transitive:</b> $$a \sim b \wedge b \sim c \rightarrow a \sim c$$

A very classic example of such equivalence relation is modular arithmetic, where, say, 1 o clock is similar to 13 o clock, where $$13 \equiv 1 \pmod{12}$$. We will discuss modular arithmetic in number theory elaborately.

## Partial Order

Partial order is not defined for all pair of elements in a set $$A$$, but when a specific property satisfies, the order establishes. The order, after establishing, is "just exists", it doesn't have to engage in any functional properties. This will be useful in our category theory discussions (Generally morphisms in categories are first defined from set-functions, so when a category is defined on posets, the notion of a function "doing something" bleeds in the partial order's understanding)

It has some special properties, namely-

- <b>Comparability:</b> Two elements a and b are comparable if $$a \le b \lor b \le a$$. If neither is true, the elements are incomparable.
- <b>Bounds:</b> $$\exists a,b$$ s.t. $$(\forall x \in A) \; x \le a$$ and $$(\forall x \in A) \; x \ge b$$. A poset can have multiple such elements.

Example: The divides relation ($$a \mid b$$) on integers. $$2 \le 6$$ and $$3 \le 6$$ but, 2 and 3 don't divide each other, so they are incomparable.

### Posets
Posets are sets that have a relation R defined on themm, and they need not to be comparable. Hasse diagrams exist to visually represent finite posets.

## Total Order

Total order is similar to partial orders but with one rule, every element is comparable. So, the trichotomy property is introduced-

-<b>Trichotomy:</b> $$(\forall x,y \in A) \; (x \le y) \lor (x \ge y) \lor (x = y)$$ (By the way, $$x = y$$ is a "diagonal" equivalence relation).

Example: The standard less than or equal to relation ($$\le$$). For any two reals the trichotomy, and other ordering properties hold.

### Strict Order
Created by dropping the reflexive property, uses $< instead of \le$$. 

### Preorders
Dropping the antisymmetric property, i.e. elements aren't identical.

## Lattices

Lattices are a fundamental construct of Order theory. A lattice is a special type of poset where every pairs have a unique 
```mermaid
graph BT
    1 --> 2
    1 --> 3
    2 --> 4
    2 --> 6
    3 --> 6
    4 --> 12
    6 --> 12
