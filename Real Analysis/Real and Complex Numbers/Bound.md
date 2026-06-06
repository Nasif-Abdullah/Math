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

![Alpha is a supremum](https://kroki.io/tikz/svg/eNqNlNtq20AQhu_1FFNwwAZJlU_pRQ4QsEoNaQNOKAXLF6vV2F68lsRKSuwKvXtnV5Zl50TBF_JoNPN__85OECW82GKcc8mybJ6LzV87TFSE6qbvpfmizHIWR0wmMVZWUGSoM6QIFVP7MkKeKJaLJM7clOVrhalkXMSrOjVlfMNWWLJtlu23YQUXcO04DtxNJv4Enn5MH-F--suHpwf4Pv1DAR_82exhZllBiCsRl422qgno5qngeaFIjXUBE8VeIF8jKGQSpIjRCiKKzZ1bO18LvllA1-nbXg-obfdSP8RJhHMlVut8AWUn2JLsMCxnVae6MhVxSVUgS7YIz0wWmFFFXAZMpmv2m8lyXNUBTDNBruhQ322CJuuniIvMr1-Xxw_BgZNvjPqfTG2gTgAyuXlsE4F-79E1aMfiNnhuv4Y8iTkmaIBDlMmLATavNex7pU6lv6l5_vLj4icAB1Mf1yxCQyLiHBX52tQ8ybUP_AsrWAop5yGZ_2Xgva_New37NuCOPhTfvON7LtEovGcEcaaw9uek4vkBfh1ofy5rB6AMsi2TEqYNXucTvtb8a-d28anAVzxG6gxThRndCiOXLiT40MUd26YSASXqC5P1yMSExoavIdgRE5SeO7ah75LsgevZMHT7NozcYWUBGL-NoJCur5mGnTn9cQ-4UOQRdAdpXrc_XjleKLkHWgScjjahGW1k-Qe6w3ZAu10TN6XJt7VYkRcR3ozTvKKGnjskwmENPSKp-s9VcwYDd6T1fGvc7viHwWq92EGXxQ0-JEsy5UXQcMdnh9qzWlaF0UL3GlLplnNInPVUszB5RhtMWtnZHfdDxpVINQyQw6Z603XXLh_9mQ26_7FHSzfUB-Gdtzk43wxSs-9YWEimqpJXcHeGRxZAEJCEghbHgZL-i_8aQArF0bG4BqsDp9vVRI4L-B8aYwe1)

![Alpha is not a supremum](https://kroki.io/tikz/svg/eNqNVNtq4zAQfc9XzEIKKdheJ2m6D73AQrxsoBdIy7IQ50GWJ4mIYhvJbpMa__uO5NhJryz4wT4aH51zpJkwTnmxwSTnkmk9y8X6xYlSFaO66vtZPi91zpKYyTTBqhMWGk2FFJFialfGyFPFcpEm2stYvlKYScZFsqxLM8bXbIkl22i920QVnMCl67rwczwOxvD4e_IAN5O7AB7v4dfkLwEBBNPp_bTTCSNciqRstFUNYDbPBM8LRWo6JzBW7BnyFYJCJkGKBDthTNjMvXbyleDrOfTcvuOfAm3bOzcvSRrjTInlKp9D2Q03JDuKymnVrS4sIy6IBXS6QXhiskBNjLgImcxW7A-T5aiqAcy0oFQM1Pca0FbdiqTQQb1ctj-CC0f_WPW3TK2hLgAKuXk9FAI9H7lrrLXkDvhevzZ5hLkWtIYjlOmzNWyXjdmPqI6lv-N8vfg5-ZGBfagPKxajdSKSHBXl2nAe1Tp7__NOuBBSziIK_9vA_1ib_9bse8A7-1R8s8Z3XKJVeMPIxCuFdT5HjK8P8PvA5HNeJwBlqDdMSpg09rpf-DuEf-lez78U-MaPlTrFTKGmrrByqSEhgB5u2SaTCCjRNIw-pRBTujZ8BeGWPEHpeyMH-h7JHni-A0OvX3UAbNRWS0Sday_C1h786BS4UBQP9AZZXu_cdhsvlNwBzQBOp5rS9WwUBXtj-8GAzmFCXJW23jE6RV7EeDXK8oo29L0hmRvWfs9Ipfm4aOIfeGdGz48m6G5g71TdqporkRlyILNW2d4_bA9zgOTFDi2KZG74h4au3W1oMmmmAovSJ3Rgn0Rzps3oYVEhmapKXsFd2m6ULoAkQRiShIJ6WNQdS9_iv-4CQUnckhtrNXA86CzSzsJ_A47hkg==)

$\blacksquare$
