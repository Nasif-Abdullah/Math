---
layout: default
title: Introduction to Topology
---

In analysis we have this notion of distance, and neighborhoods building upon them that allows us define important notions like open sets, closed sets etc. In real analysis, real numbers are complete, have "no holes" so we can define any values of distance using them.

Unfortunately there exist many branches of math where one doesn't get the privilege to use real numbers to define distances, like if we have a set $$S = \{alice, bob, cameroon\}$$, how would you define a "distance" or an "open set" within the set $$S$$? Through decades of abstraction, mathematicians could finally throw away the "ruler" to define such notions, which gave birth to topology.

Topology is basically like a "rule of the club" where you take any set, addresses its elements and check if these elements satisfy some conditions or axioms, which creates a topology.

Take any set $$X$$ and define $$\tau = \{U \mid U \subseteq X \wedge \phi(U)\}$$ Where $$\phi(U) \iff (\phi(\emptyset) = T \wedge \phi(X) = T) \wedge ((\forall i \in I) \ \ \phi(U_i) \rightarrow \phi(\bigcup_{i \in I} U_{i})) \wedge ((\forall i \in \{1,...n})(\bigwedge_{i=1}^n \phi(U_i)) \rightarrow \phi(\bigcap_{i=1}^{n} U_{i})$$

Note, the set-builder only picks up subsets of the set $$X$$ so it's a valid set-builder and won't explode into any set-theoretic inconsistencies. Obviously, $$\tau$$ is a collection of sets.

A topological space is the ordered pair $$(X, \tau)$$. If for any $$U \subset X$$ we have $$U \in \tau$$, we say $$U$$ is an open set. The naming is completely arbitrary here.

We now begin with a simple example on what can and can't be a topology. 

Take a set $$X = \{a,b,c\}$$, and it's subsets, $$U_i \subseteq X$$ and the $$U_i$$ are, in order, the following sets- $$\{a\}, \{b\}, \{c\}, \{a,b\}, \{b,c\}, \{a,c\}, \{a,b,c\}, \emptyset$$. We assume $$\phi(U_i) = T$$ so we construct the collection, $$\tau = \{\{a\}, \{b\}, \{c\}, \{a,b\}, \{b,c\}, \{a,c\}, \{a,b,c\}, \emptyset\}$$ Now we check if it forms a topology-

 - $$(\phi(\{a,b,c\}) = T) \wedge (\phi(\emptyset) = T)$$ By assumption.
 - By assumption $$(\forall i \in I) \ \ \phi(U_i) = T$$ so we have the following unions- $$\bigcup_{i \in I} (U_i) \in \tau$$ so $$\phi(\bigcup_{i \in I} (U_i)) = T$$ (The rbitrary union of any subsets of a power set is within the power set. So every union represents a $$U_i$$ for an $$i \in I$$, but we have assumed that $$\phi(U_i) = T$$ for any $$i$$, so the union satisfies the predicate.)
 - And  $$(\forall i \in I) \ \ \phi(U_i) = T$$ so we have the following finite intersection- $$\bigcap_{i=1}^{n} (U_i) \in \tau$$ so $$\phi(\bigcap_{i = 1}^{n} (U_i)) = T$$ (Note, empty set is also in the collection).

So the assumption holds and the collection forms a topology on $$X$$. This is an elementary topology called the discrete topology, when the collection is the power set of a set $$X$$.

Meanwhile, if the collection was constructed like $$\tau = \{\{a\}, \{b\}, \{c\}, \{a,b\}, \{a,c\}, \{a,b,c\}, \emptyset\}$$, union of $$\{b\}$$ and $$\{c\}$$ is not present in the collection, so the collection $$\tau$$ is not a topology.

From now on we will have $$\phi(U) \iff \phi(U) = T$$ from set theory notations. This will keep the prose economic.

## Trivial Topology
For any set $$X$$, $$\tau = \{X, \emptyset\}$$ forms the trivial topology, which can be proven trivially. 
Refering to the previous example, we have $$X = \{a,b,c\}$$. Now, let $$\tau$$ be the trivial topology, and $$\tau^{\mathfrak{B}}$$ be the discrete topology. Obviously, $$(\forall i \in I) (U_i \in \tau) \implies (U_i \in \tau^{\mathfrak{B}})$$, so $$\tau \subseteq \tau^{\mathfrak{B}}$$. Then $$\tau$$ is "coarser" than $$\tau^{\mathfrak{B}}$$, and $$\tau^{\mathfrak{B}}$$ is "finer" than $$\tau$$. If the containment is proper, we have strictly finer or strictly coarser topologies.

If for any two topologies such containment can be established, we call them comparable.

## Cofinite topology

Let X be an infinite set and we have $$U \subseteq X$$ .We define the predicate as $$\phi(U) \iff (U = \emptyset) \lor Finiteness(X \setminus U)$$. This roughly translates to "$$U \subseteq X$$ is open iff it's complement is finite or it is the empty set.

If a set $$U$$ is finite, here, $$Finiteness(U) = T$$. Now we have-

 - $$(U = X) \rightarrow \phi(U)$$ as $$Finiteness(X \setminus X)$$ (which is just the empty set). And $$(U = \emptyset) \rightarrow \phi(U)$$ (by definition)
 - Assume $$(\forall i \in I)\ \ \phi(U_i)$$. Now if all $$U_i = \emptyset \rightarrow \bigcup_{i \in I} (U_i) = \emptyset$$, and if $$(\exists j \in I) \ \ U_j \neq \emptyset$$. Now as we assumed $$\phi(U_i)$$ and $$U_i \neq \emptyset$$, so $$Finiteness(X \setminus U_j)$$ holds. Now we have, $$X \setminus (\bigcup_{i \in I}) = \bigcap_{i \in I} (X \setminus U_i)$$, and intersection of finite sets is finite so, $$\phi(\bigcup_{i \in I} U_i)$$ holds.
 - Similarly, assume $$(\forall i \in I) \ \ \phi(U_i)$$. If $$\exists i$$ such that $$U_i = \emptyset$$, then $$\bigcap_{i=1}^n U_i = \emptyset \implies \phi(\bigcap_{i=1}^n U_i)$$. Otherwise, $$(\forall i) \ \ Finiteness(X \setminus U_i)$$ holds. Now, $$X \setminus \left(\bigcap_{i=1}^n U_i\right) = \bigcup_{i=1}^n (X \setminus U_i)$$ (De Morgan). Since a finite union of finite sets is finite, $$\phi(\bigcap_{i=1}^n U_i)$$ holds. 

So, $$\tau$$ is a topology.
$$\square$$
