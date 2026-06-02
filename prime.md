# Pure Mathematics Notes

## Theorem: Infinitude of Primes
There are infinitely many prime numbers.

### Proof (Euclid)
Suppose for contradiction that there is a finite number of primes, which we can list completely as:
$$P = \{p_1, p_2, \dots, p_n\}$$

Consider the integer $N$ constructed by multiplying all these primes together and adding $1$:
$$N = (p_1 \cdot p_2 \cdot \dots \cdot p_n) + 1$$

By the Fundamental Theorem of Arithmetic, $N$ must have at least one prime factor, let's call it $q$. 

Since our list $P$ contains *all* prime numbers, $q$ must be one of the primes in our list (i.e., $q = p_i$ for some $1 \le i \le n$). Therefore, $q$ cleanly divides the product:
$$q \mid (p_1 \cdot p_2 \cdot \dots \cdot p_n)$$

However, by definition, $q$ also divides $N$. This implies that $q$ must divide the difference:
$$q \mid [N - (p_1 \cdot p_2 \cdot \dots \cdot p_n)]$$

Since $N - (p_1 \cdot p_2 \cdot \dots \cdot p_n) = 1$, we conclude that:
$$q \mid 1$$

But no prime number can divide $1$, creating a **contradiction**. 

Thus, the initial assumption that there are finitely many primes must be false. $\blacksquare$
