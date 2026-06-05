---
layout: default
title: Newton's Method 
---

Newton's method, or newton-raphson method, is an iterative numerical algorithm to find succesively better approximations to a root or zeros of a function, $$f(x) = 0$$.

Let $$x_n$$ be the current approximation of the root of the function, $$f(x)$$. So, the corresponding point of the function is $$(x_n, f(x_n))$$. Now, the slope at that point, $$x_n$$ is the derivative of the function evaluated at that point- $$m = f^{i} (x_n)$$

So we have, $$y - f(x_n) = f^{i} (x_n) (x - x_n)$$, being the equation of the tangent line. The next approximation is determined, $$x_{n+1}$$ to be the point where the line crosses x axis, so, $$(y = 0) \wedge (x = x_{n+1})$$

and from algebraic manipulation we have- 

$$ x_{n + 1} = x_n - \frac{f(x_n)}{f^{i} (x_n)} $$

This method was used to find the q from the <a href = "../Real Analysis/Introduction.html#i">analysis note</a>, and we'll discuss how now-

We desire to find the solution to the equation- $$p^2 - 2 = 0$$. As it's in the form of $$f(p) = 0$$, we can use newton's method. We calculate the derivative, for $$f(p) = p^2 - 2, f^{i} (p) = 2p$$

and from that, we have, $$q = p_{n + 1}$$ (and set $$p_n = p$$) and

$$q = p - \frac{p^2 - 2}{2p}$$.

We simplify the expression to get-

$$q = \frac{p}{2} + \frac{1}{p}$$

And we have, $$q^2 - 2 = \frac{(p^2 - 2)^2}{4 p^2}$$

Notice, the numerator, $$(p^2 - 2)^2$$ is squared, so it's always positive, so $$q^2$$ is always greater than $$0$$. So we couldn't find a $$q$$ such that $$(p^2 < 2) \rightarrow (q^2 < 2) \wedge (q > p)$$, i.e. the equation from newton's method to find q oversteps or understeps when p is in A and B, respectiely. (Recall, $$A = \{p \in \mathbb{Q} \mid p^2 < 2 \}$$ and $$B = \{p \in \mathbb{Q} \mid p^2 > 2 \}$$) 

So we modify the equation- for the value of q is disproportionate to the value of it's expression's denominator.

Now we replace the denominator $$2p$$ by some $$p + k$$ in the expression- $$ q = p - \frac{p^2 - 2}{2p} $$.

We get- $$ q = p - \frac{p^2 - 2}{p + k} $$.

Now setting $$k = 2$$ produces the equation used in the analysis note.

(It is to be noted that, if we could prove that the overstepping or understepping was bound to happen, we wouldn't have to construct reals anymore)


