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
$$\frac{d}{dx} ln(x) = \frac{1}{x}$$
$$\frac{d}{dx} sec(x) = \frac{sin(x)}{cos^2(x)}$$
$$\frac{d}{dx} csc(x) = \frac{cos(x)}{sin^2(x)}$$

### Product and Quotient Rule

$$\frac{d}{dx} f(x)g(x) = f'(x)g(x) + f(x)g'(x)$$
$$\frac{d}{dx} \frac{f(x)}{g(x)} = \frac{f'(x)g(x) - f(x)g'(x)}{g(x)^2}$$


## Unit 3: Composite, Implicit, Inverse differentiation

### Implicit differentiation

Since the relation implies y is some function of x, we can set $y = f(x)$ and differentiate with the chain rule.

### Inverse differentiation

$$f(f^{-1}(x)) = x$$
$$\frac{d}{dx} f(f^{-1}(x)) = \frac{d}{dx} x$$
$$f'(f^{-1}(x))[f^{-1}(x)]' = 1$$
$$[f^{-1}(x)]' = \frac{1}{f'(f^{-1}(x))}$$

### Log/Exponential of different bases

$$\frac{d}{dx} log_b(x) = \frac{1}{x \cdot ln(b)}$$
$$\frac{d}{dx} a^x = ln(a)\cdot a^x$$

### Composite differentiation

Pick the easiest way to differentiate. For example $(x^2+2)^2 = x^4 + 4x^2 + 4$, which is easily differentiable by the power rule. 

### Second derivatives

Take the derivative of the derivative, and plug back in as needed. Be careful with algebra!


## Unit 4: Miscellaneous Derivative

### Motion graphs


### Related Rates

Set up an equation, and just do it.

### Local approximation

Say we want to approximate $f(c)$. Choose a point close to c, find the derivative at that point, and write up a linear equation. Then, simply plug $c$ to approximate.

### L'hopital's Rule
The limit of an indeterminate form ($\frac{0}{0}, \frac{\infty}{\infty}$) is equal to the limit of the derivatives of the numerator and denominator.


## Unit 5: Analyzing functions using derivatives

### Mean Value Theorem

For any continuous, differentiable function in the range $[a, b]$, there exists a number $c$ that $f'(c)$ is equal to the averange rate of change (slope) over $[a, b]$.

### Extreme Value Theorem

For a continuous function over the range $[a, b]$, there must exist a maximum and minimum value. These values are at critical points or endpoints.

A critical point is a point at which the derivative of the function is either zero or undefined.

### Concavity 

