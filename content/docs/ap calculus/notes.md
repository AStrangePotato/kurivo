---
title: Notes
weight: 1
---

## Unit 1: Limits and Continuity

The limit $\lim_{x \to a} f(a)$ exists if the limit from the left is the same as the limit from the right. 

If the left and right limits approach the same thing, it could be unbounded (tends to $\pm\infty$). 

If the left and right limits do not approach the same thing, then the limit does not exist.

A function is continuous at $a \iff \lim_{x \to a} f(x) = f(a)$.


### Limit Properties

$$\lim_{x \to p} (f(x) + g(x)) = \lim_{x \to p} f(x) + \lim_{x \to p} g(x)$$
$$\lim_{x \to p} (f(x) - g(x)) = \lim_{x \to p} f(x) - \lim_{x \to p} g(x)$$
$$\lim_{x \to p} (f(x) \cdot g(x)) = \lim_{x \to p} f(x) \cdot \lim_{x \to p} g(x)$$
$$\lim_{x \to p} \left(\frac{f(x)}{g(x)}\right) = \frac{\lim_{x \to p} f(x)}{\lim_{x \to p} g(x)}$$




### Discontinuities
 - Point/removable discontinuity
 - Jump discontinuity
 - Asymptotic discontinuity

### Continuity over an interval
Function f is continuous over $(a, b)$ if and only if $\lim_{x \to c} f(x) = f(c)$ for all $a < x < b$.
F is continuous over $[a, b]$ if and only if f is continuous over $(a, b)$ and the right handed limit at a is equal to $f(a)$, and the left handed limit at b is equal to $f(b)$.

### Intermediate Value Theorem
If a function is continuous over all values in $[a, b]$ then the function must take on every value between $f(a)$ and $f(b)$ at least once.

### Squeeze Theorem

### Other Common Limits
$$\lim_{x \to 0} \frac{sin(x)}{x} = 1$$
$$\lim_{x \to 0} \frac{e^x - 1}{x} = 1$$


## Unit 2: Definition and basics of derivatives

Standard form: $\lim_{h \to 0} \frac{f(x+h)-f(x)}{x+h-h}$  
Alternate form: $\lim_{c \to x} \frac{f(c)-f(x)}{c-x}$ (simply set $c = x+h$)

If f is differentiable at c, then f is continuous at c. If f is not differentiable at c, then f is not continous at c. Note continuity does not imply differentiability.

### Common derivatives

$$\frac{d}{dx} sin(x) = cos(x)$$
$$\frac{d}{dx} cos(x) = -sin(x)$$
$$\frac{d}{dx} tan(x) = sec^2(x)$$
$$\frac{d}{dx} cot(x) = -csc^2(x)$$
$$\frac{d}{dx} e^{x} = e^{x}$$
$$\frac{d}{dx} ln(x) = 1/x$$
$$\frac{d}{dx} sec(x) = \frac{sin(x)}{cos^2(x)}$$
$$\frac{d}{dx} csc(x) = \frac{cos(x)}{sin^2(x)}$$


### Product and Quotient Rule

$$\frac{d}{dx} f(x)g(x) = f'(x)g(x) + f(x)g'(x)$$
$$\frac{d}{dx} \frac{f(x)}{g(x)} = \frac{f'(x)g(x) - f(x)g'(x)}{g(x)^2}$$

### Implicit differentiation

Since the relation implies y is some function of x, we can set $y = f(x)$ and differentiate with the chain rule.