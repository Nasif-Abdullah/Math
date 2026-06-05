---
layout: default
title: Newton's Method 
---

Newton's method, or newton-raphson method, is an iterative numerical algorithm to find succesively better approximations to a root or zeros of a function, $$f(x) = 0$$.

Let $$x_n$$ be the current approximation of the root of the function, $$f(x)$$. So, the corresponding point of the function is $$(x_n, f(x_n))$$. Now, the slope at that point, $$x_n$$ is the derivative of the function evaluated at that point- $$m = f^{'} (x_n)$$

So we have, $$y - f(x_n) = f^{'} (x_n) (x - x_n)$$, being the equation of the tangent line. The next approximation is determined, $$x_{n+1}$$ to be the point where the line crosses x axis, so, $$(y = 0) \wedge x = x_{n+1}$$

and from algebraic manipulation we have- 

$ x_{n + 1} = x_n - \frac{f(x_n)}{f^{'} (x_n)} $

