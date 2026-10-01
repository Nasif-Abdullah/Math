---
layout: default
title: Continuity of functions
---

Continuous functions are a central study of Real Analysis. In metric spaces, continuous functions are defined with the $\epsilon - \delta$ argument, and this can be outlined as follows-

In a metric space $(M,d)$, a function $f$ is continuous at a point $x$ if $\forall \epsilon >0 ~ \exists \delta >0$ such that for any $y \in M, d(x,y)<\delta \implies d(fx, fy)<\epsilon$

The definition have some logical properties-
 
 - We first choose an $\epsilon >0$. The definition suggests that any values of epsilon should satisfy the implications. After choosing any $\epsilon$, like $\epsilon = 1$, 
 - We find a $\delta > 0$ such that the implication holds. For any $\delta$ which we claim to satisfy the implication, for any point $y \in N_{\delta} (x)$ we must have $d(fx, fy)<\epsilon$ for the chosen epsilon.
 - For the points $y$ such that $y \in M / N_{\delta} (x)$, the logical implication is vacuously true ($P(F \implies T) = T$). 