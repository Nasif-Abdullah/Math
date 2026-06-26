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

A topological space is the ordered pair $$(X, \tau)$$. If for any $$U \subset X$$ we have $$U \in \tau$$, we say $$U$$ is an open set. The naming is completely arbitrary here.

We now begin with a simple example on what can and can't be a topology. 

Take a set $$X$$ = $$\{a,b,c\}$$, and we take the following subsets, $$U_i \in X$$ and the $$U_i$$'s are, in order, the following sets- $$\{a\}, \{b\}, \{c\}, \{a,b\}, \{b,c\}, \{a,c\}, \{a,b,c\}, \emptyset$$. We assume $$\phi(U_i) = T$$ so we construct the collection, $$\tau = \{\{a\}, \{b\}, \{c\}, \{a,b\}, \{b,c\}, \{a,c\}, \{a,b,c\}, \emptyset\}$$ Now we check if it forms a topology-

 - $$(\phi(\{a,b,c\}) = T) \wedge (\phi(\emptyset) = T)$$ By assumption.
 - By assumption $$(\forall i \in I) \ \ \phi(U_i) = T$$ so we have the following unions- $$\bigcup_{i \in I} (U_i) \in \tau$$ so $$\phi(\bigcup_{i \in I} (U_i)) = T$$ (Arbitrary union of any subsets of a power set is within the power set. So every union represents a $$U_i$$ for an $$i \in I$$, but we have assumed that $$\phi(U_i) = T$$ for any $$i$$, so the union satisfies the predicate.)
 - And  $$(\forall i \in I) \ \ \phi(U_i) = T$$ so we have the following finite intersection- $$\bigcap_{i=1}^{n} (U_i) \in \tau$$ so $$\phi(\bigcap_{i = 1}^{n} (U_i)) = T$$ (Note, empty set is also in the collection).

So the assumption holds and the collection forms a topology on $$X$$. This is an elementary topology called the discrete topology, when the collection is the power set of a set $$X$$.

Meanwhile, if the collection was constructed like $$\tau = \{\{a\}, \{b\}, \{c\}, \{a,b\}, \{a,c\}, \{a,b,c\}, \emptyset\}$$, union of $$\{b\}$$ and $$\{c\}$$ is not present in the collection, so the collection $$\tau$$ is not a topology.

From now on we will have $$\phi(U) \iff \phi(U) = T$$ from set theory notations. This will make the prose economic too.

## Cofinite topology

Let X be an infinite set and we have $$U \subseteq X$$ .We define the predicate as $$\phi(U) \iff (U = \emptyset) \lor Finiteness(X \setminus U)$$. This roughly translates to "$$U \subseteq X$$ is open iff it's complement is finite or it is the empty set.

If a set $$U$$ is not finite, here, $$Finiteness(U) = T$$. Now we have-

 - $$(U = X) \rightarrow \phi(\tau)$$ as $$Finiteness(X \setminus X)$$ (which is just the empty set). And $$(U = \emptyset) \rightarrow \phi(U)$$ (by definition)
 - Assume $$(\forall i \in I)\ \ \phi(U_i)$$. Now if all $$U_i = \emptyset \rightarrow \bigcup_{i \in I} (U_i)$$ (as it will just be the empty set), and if $$(\exists j \in I) \ \ U_j \neq \emptyset$$. Now as we assumed $$\phi(U_i)$$ and $$U_i \neq \emptyset$$, so $$Finiteness(X \setminus U_j)$$ holds. Now we have, $$X \setminus (\bigcup_{i \in I}) = \bigcap_{i \in I} (X \setminus U_i)$$, and intersection of finite sets is finite so, $$\phi(\bigcup_{i \in I}) U_i)$$ holds.
 - Similarly, finite union of finite sets is finite, so the intersection property holds (De-Morgan).

So, $$\tau$$ is a topology.
