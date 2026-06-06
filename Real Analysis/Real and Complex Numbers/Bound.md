---
layout: default
title: Boundedness of Real Numbers
---

### Bound

Suppose $$S$$ is an ordered set, and $$E \subseteq S$$. If $$\exists B \in S$$ such that $$(\forall x \in E) \ \ x \le B$$ we say $$E$$ is bounded above, and call $$B$$ is an upper bound of E.

Note, $$B$$ is in the "parent set", $$S$$, so the upper bound can exist outside of the subset we are dealing with.

Similarly, $$L$$ is a lower bound when $$(\forall x \in E)\ \ (\exists L \in S) \ \ x \ge L$$.

Define the set, $$UB = \{x \in S \mid (\forall e \in E) \ \ x \ge e \}$$. This set contains all upper bounds of E. A similar set can be constructed to set all lower bounds of E, call it $$LB = \{x \in S \mid (\forall e \in E) \ \ x \le e \}$$

### Supremum and Infimum

Supremum, or the least upper bound, can be defined as, $$\alpha = sup \ \ E = min(UB)$$. Similarly, $$\beta = inf \ \ E = max (LB)$$.

Some properties of the least upper bound-

 - Supremum may or may not be an element of E, as evident from the set construction. Set $$E = 1/n, n \in \mathbb{N}$$. Now the supremum is $$1$$, which is in $$E$$, but the infimum is zero, which is not in E. Another concrete example can be of a set $$E$$, defined as $$E = \{x \in \mathbb{Q} \mid x \le 0\}$$, then the supremum would be $$0$$ which is not in $$E$$. (Notice, how no member of the set $$E$$ can be a supremum, there are no largest number in $$E$$. For any hypothesized largest number $$q$$, we have $$\frac{q + 0}{2} = q^{'}, q^{'} > q$$ for $$q$$ is a negative number. But, this logic can be used in any subset of rationals, and we call these subsets open sets, which will be discussed later.

 - If we hypothesize $$\alpha$$ to be the supremum of set $$E$$ but there exists any $$\epsilon > 0$$ s.t. $$(\alpha - \epsilon) \in UB$$ then $$\alpha$$ would not be the supremum. This can be rephrased as, if $$(\nexists x \in E) \ \ \alpha - \epsilon < x < \alpha$$, then $$\alpha$$ wouldn't be the supremum. This seemingly simple concept will be used many times througout analysis, and we included a diagram for this.


![Alpha is a supremum](https://kroki.io/tikz/svg/eNqNVNtq20AQffdXzIMDDkiqfEsfcoGAVWpIGnBDKUR-WElje_Hqwu4qcSL0751dXew0KRT0IJ2dPXPO2R2FSR6XKWY6FkypJ833b06UywTl9dgv9LpSmmUJE3mG9SAsFZoKwSPJ5GuVYJxLpnmeKa9geiexECzm2bYpLVi8Z1usWKrUaxrVcAZXruvC7WIRLODx-_In3C1_BPD4AN-WvwkIIFitHlaDQRjhlmdVp63uANO84LEuJakZnMFCshfQOwSJTIDgGQ7ChLAn98bROx7v1zByx45_DtR2dGFesjzBJ8m3O72GahimJDuKqlU9rC8tI26IBVSeIjwzUaIiRtyETBQ79ouJal43ABaKUyoGGnsdaKvueVaqoFmu-o3gwskeq_6eyT00BUAhd6_HQqDnM3edtZ7cAd8bNyZPMNeC1nCEIn-xhu2yMfsZ1an0D5zvF_9NfmKgDfWOUYl1wjONknJtup-ofR_Pl4npftHwQxWqlAkBy3YzDEcfOjlteuujtSv35nNjvjf7OysDWakrLCQqunNWLl13CGCEB5YWAgEFmuuozgfhJqdDiXcQHsgTVL43d2DskeyJ5zsw9cYOzLxpPQAIN1wIKyii4bBZH2y283OIuYyJdzQpdNO-v9BxKcUr0JjFCDqnG9DJClp37eyhcxzC68rWO0Ys12WC1_NC19TQ96bkcNqYnpFU83HZncHEmxk9X7u0h0E_CyqWvDDUQH6trjYCOBwHjcQlDi3ybG3Yp4as7zU1sXRjx6L8GR1oc-iOtZttFpWCybqKa7jN-kb5BkgQhCFJKGlIeDMS9M3_6zoQlCU9uTHWAKd_Eov0P5s_EH6u4A==)

![Alpha is not a supremum](https://kroki.io/tikz/svg/eNqNVF1r2zAUffevuA8ppGB7TtJ0D_2AQTwWaFfIyhjUeZDtm0RE_kCS23TG_31X8kfStYOBH-yjq3PPOdJ1lBZJlWGuE8GUetJ8_9uNC5mivJkEpV7XSrM8ZaLIsXGiSqGpEDyWTL7WKSaFZJoXufJLpncSS8ESnm_b0pIle7bFmmVKvWZxA2dw7XkefFkswgU8flv-gLvl9xAeH-Dr8hcBIYSr1cPKcaIYtzyve21ND5jmJU90JUmNcwYLyV5A7xAkMgGC5-hEKWFP3q2rdzzZr2HsTdzgHKjt-NK85EWKT5Jvd3oN9SjKSHYc16tm1FxZRtwQC6giQ3hmokJFjLiJmCh37CcT9bxpASwVp1QMNPF70Fbd87xSYbtcDxvBg5M9Vv09k3toC4BC7l-PhUDPR-56awO5C4E_aU2eYJ4FreEYRfFiDdtlY_YjqlPp7zjfLv6b_MRAF-odoxLrhOcaJeXadj9R-zaeT1PT_bLlhzpSGRMClt1mGI3fdXK79NZHa9fe7cfGAv_i76wMZKWusJSo6M5ZuXTdIYQxHlhWCgQUaK6jOneiTUGHkuwgOpAnqAN_7sLEJ9lTP3Bh5k8aByDacCGslpjmwsZ8sLHOzyHhMiHK8bTUbefhLieVFK9AE5Yg6IIOv1cUdsa6sUP3OH83ta13jU6uqxRv5qVuqGHgz8jcrPV7QSrNx1Uf_9S_MHo-90GPwmEMVCJ5aaiBrFpdnXs4HGeMxKUuLfJ8bdhnhmzoNTOJ9BPH4uIZXehy6E-0H2sWV4LJpk4a-F4MjYoNkCCIIpJQ0Xzwdhrom__XTSAoTwdyY6wFTn8iFhn-M38A9WauDQ==)


### 1.1 Theorem



$\blacksquare$
