---
layout: default
title: Introduction to Topology
---

In analysis we have this notion of distance, and neighborhoods building upon them that makes us define important notions like open sets, closed sets etc. We have, in real analysis, real numbers, which are complete, have "no holes" so we can define any values of distance using them.

Unfortunately there exists many branches of math where one don't get the priviledge to use real numbers to define distances, like if we have a set $$S = \{alice, bob, cameroon\}$$ how would you define a "distance", or an "open set" within the set $$S$$? Upon careful observations for years, mathematicians could finally throw away the "ruler" to define such notions, which gave birth to topology.

Topology is basically like a "rule of the club" where you take any set, address it's elements and check if these elements satisfy some conditions or axioms, which creates a topology.

Take any set $$X$$ and define $$\tau = \{U \mid U \subset X \wedge \phi(U) = T\}$$ When the properties, $$\phi(U)$$, are listed below-

 - $$\phi(\emptyset) = T$$ and $$\phi(X) = T$$.
 - $$\phi(U_i) = T \rightarrow \phi(\bigcup_{i \in I} U_{i}) = T$$ (and $$I$$ is any indexing set)
 - $$\phi(U_i) = T \rightarrow \phi(\bigcap_{i=1}^{n} U_{i}) = T$$ for any $$n \in \mathbb{N}$$

Note, the set-builder only picks up subsets of the set $$X$$ so, it's a valid set-builder and won't explode to any set-theoric inconsistencies. Obviously, $$\tau$$ is a collection of sets.

A topological space is the ordered pair $$(X, \tau)$$. If for any $$U \in X U \in \tau$$, we can $$U$$ an open set. The naming is completely arbitrary here.

We now begin with a simple example on what can and can't be a topology. 

Take a set $$X$$ = $$\{a,b,c\}$$, and we take the following subsets, $$U_i \in X$$ and the $$U_i$$'s are, in order, the following sets- $$\{a\}, \{b\}, \{c\}, \{a,b\}, \{b,c\}, \{a,c\}, \{a,b,c\}, \emptyset\$$. We assume $$\phi(U_i) = T$$ so we construct the collection, $$\tau = \{\{a\}, \{b\}, \{c\}, \{a,b\}, \{a,c\}, \{a\}, \{a,b,c\}\}$$ Now we check if it forms a topology-

 - $$(\phi(\{a,b,c\}) = T) \wedge (\phi(\emptyset) = T)$$ By assumption.
 - By assumption $$(\forall i \in I) \ \ \phi(U_i) = T$$ so we have the following unions- $$\bigcup_{i \in I} (U_i) \in \tau$$ so $$\phi(\bigcup_{i \in I} (U_i)) = T$$ (Works because the union is in $$\tau$$ and every element of $$tau$$ satisfies the predicate by assumption. One can check it holds for every two or more elements)
 - And  $$(\forall i \in I) \ \ \phi(U_i) = T$$ so we have the following finite intersection- $$\bigcap_{i \in I}^{n} (U_i) \in \tau$$ so $$\phi(\bigcap_{i \in I}^{n} (U_i)) = T$$ (Note, empty set is also in the collection).

So the assumption holds and the collection forms a topology on $$X$$. This is an elementary topology called the discrete topology, when the collection is the power set of a set $$X$$.

From now on we will have $$\phi(U) \iff \phi(U) = T$$ from set theory notations. This will make the prose economic too.
