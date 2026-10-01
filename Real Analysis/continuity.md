---
layout: default
title: Continuity of functions
---

Continuous functions are a central study of Real Analysis. In metric spaces, continuous functions are defined with the $\epsilon - \delta$ argument, and this can be outlined as follows-

In a metric space $(M,d)$, a function $f$ is continuous at a point $x$ if $\forall \epsilon >0 ~ \exists \delta >0$ such that for any $y \in M, d(x,y)<\delta \implies d(fx, fy)<\epsilon$

The definition have some logical properties-
 
 - We first choose an $\epsilon >0$. The definition suggests that any values of epsilon should satisfy the implications. After choosing any $\epsilon$, like $\epsilon = 1$, 
 - We find a $\delta > 0$ such that the implication holds. For any $\delta$ which we claim to satisfy the implication, for any point $y \in N_{\delta} (x)$ we must have $d(fx, fy)<\epsilon$ for the chosen epsilon.
 - For the points $y$ such that $y \in M / N_{\delta} (x)$, the logical implication is vacuously true ($F \implies T \equiv T$). 

![Continuity with Epsilon-Delta](https://kroki.io/tikz/svg/eNp1U02P2jAQvfMr5sBKQU1cEqDaVcVKPfSOVKkXwsHYA7EwdmQbSBvx32s74WvL-jTjmff87DcuuWaHPSrHJLW2pcYJJvE8KA8Wa8p2dIutE7u_jzt0b_fUVefBoFzjVqj2wnLbCaBaMHcweF5aRiXOc1Kk8D63Dql01WoAfr3AjwZtDEtu6GmZvafgKsF2K0iyPIXxCLIMkm8xUprj0oht5VbQDpvh-fsnyHEKWd4hfTghsx5L1_qIAfsnYHsFv_ZauwrYwRwRNkkzuiO9IxwHFkKAaeWMlhYSL68gxQio4pAUZJZCTl5jTzIJWfGhfxo3rwifTLruWShMfOGqaaGFcqBVrypp0qisl8a0Nlwo6nxl4dnc9cD-QTZCyqA_lpkw3lMvl8xqdzviNwazqQRObYX8q9VScJBCIXB9UuA0NBltxL07Xesq0obHjaeOb5wdADzvzsZLSrpGaZ88aIck-R1PFtPokwfp0xOPL-iCvN6hY_YRPS_qOCVZyVE6-pxnGkbyyhOzz3i-3Hj6y_6srZDeIoV-ItfaVFp7V2tq_Eeo0KIdBQN92JtIjT74J6mjtYtOTTgn-leQtzAbYz9jbemwcetNm5wvoq9tU5L_1zZ6aOtmfD4NqgPCO9UOy6NX1cmNFyhR8Ycv2m_d_vE_PjM0Cg==)