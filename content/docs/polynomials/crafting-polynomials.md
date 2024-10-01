---
title: Crafting Polynomials
weight: 1
---

# Some interesting problems

$$
\text{For} \; n \geq 2 \; \text{the polynomial} \;
P_n(x) = x^n + a_{n-1}x^{n-1} + \dots + a_1x + a_0 \;
\text{has the property that} \;
P_n(k) = 5k^{n-1} \;
\text{for} \; k = 1, 2, \dots, n.
$$

$$
\text{Find an expression for} \; a_{n-1} \; \text{in terms of} \; n.
$$

---

Hint: Consider crafting a polynomial $g(x)$ with roots at 1, 2, 3, ... n.

Let $g(x) = P_n(x) - 5x^{n-1}$
Thus, $g(x) = 0$ for x = 1, 2, 3 ... n.
Since it has these roots, we can express it in factored form as $(x-1)(x-2)(x-3)...(x-n)$.

$(x-1)(x-2)(x-3)...(x-n) = P_n(x) - 5x^{n-1}$

Observe the left hand side's coefficient is $-(1+2+3+ \dots +n) = -n(n+1)/2$.

Matching coefficients, 
$$
-n(n+1)/2 = a_{n-1} - 5
$$
$$
a_{n-1} = \boxed{5 - n(n+1)/2}
$$
