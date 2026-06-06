---
layout: default
title: Boundedness of Real Numbers
---

### Bound

Suppose $$S$$ is an ordered set, and $$E \subset S$$. If $$\exists B \in S$$ such that $$(\forall x \in E) \ \ x \le B$$ we say $$E$$ is bounded above, and call $$B$$ is an upper bound of E.

Note, $$B$$ is in the "parent set", $$S$$, so the upper bound can exist outside of the subset we are dealing with.

Similarly, $$L$$ is a lower bound when $$(\forall x \in E)\ \ (\exists L \in S) \ \ x \ge L$$.

Define the set, $$UB = \{x \in S \mid (\forall e \in E) \ \ x \ge e \}$$. This set contains all upper bounds of E. A similar set can be constructed to set all lower bounds of E, call it $$LB = \{x \in S \mid (\forall e \in E) \ \ x \le e \}$$

### Supremum and Infimum

Supremum, or the least upper bound, can be defined as, $$\alpha = sup \ \ E = min(UB)$$. Similarly, $$\beta = inf \ \ E = max (LB)$$.

Some properties of the least upper bound-

 - Supremum may or may not be an element of E, as evident from the set construction. Set $$E = 1/n, n \in /mathbb{N}$$. Now the supremum is $$1$$, which is in $$E$$, but the infimum is zero, which is not in E. Another concrete example can be of a set $$E$$, defined as $$E = \{x \in \mathbb{Q} \mid x \le 0\}$$, then the supremum would be $$0$$ which is not in $$E$$. (Notice, how no member of the set $$E$$ can be a supremum, there are no largest number in $$E$$. For any hypothesized largest number $$q$$, we have $$\frac{q + 0}{2} = q^{'}, q^{'} > q$$ for $$q$$ is a negative number. But, this logic can be used in any subset of rationals, and we call these subsets open sets, which will be discussed later. 
 - If we hypothesize $$\alpha$$ to be the supremum of set $$E$$ but there exists any $$\epsilon > 0$$ s.t. $$(\alpha - \epsilon) \in UB$$ then $$\alpha$$ would not be the supremum. This can be rephrased as, if $$(\nexists x \in E) \ \ \alpha - \epsilon < x < \alpha$$, then $$\alpha$$ wouldn't be the supremum. This seemingly simple concept will be used many times througout analysis, and we included a diagram for this. 

$\blacksquare$
