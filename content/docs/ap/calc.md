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

A section is concave upwards if the derivative is increasing over that interval. Concave downwards if decreasing over that interval.

For concave upwards, the second derivative is positive. Concave downwards, the second derivative is negative.

The *possible* inflection points happen when the second derivative is zero or undefined. However, these are just candidates - an actual inflection point must be when the second derviative changes signs. Remember to also check the original function is defined for this candidate point.

### Optimization

Just setup up an equation and be careful, check both endpoints, defined in original function, ...


## Unit 6: Integration and Accumulation of change

### Riemann sums

Left, right, midpoint, trapezoidal Riemann sums. Use in place of integration when function is difficult to integrate.

### Fundamental Theorem of Calculus

$$\frac{dF}{dx} = \frac{d}{dx}\int_{a}^{x}f(t)dt = f(x) $$
Every continuous function $f$ has an anti-derivative $F$.

### Properties of Definite Integrals

Area below curve is negative area.

Integral of a line is 0.

You can take out the constant in an integral.

Swapping bounds of integration results in the negative of the value.

Integral of a sum of functions is the sum of the integrals of the functions.

You can break apart integrals.

### Rules of integration

$\int x^n dx = \frac{x^{n+1}}{n+1} + C$

$\int cf(x) dx = c \int f(x) dx$

$\int(f(x) + g(x))dx = \int f(x) dx + \int g(x) dx$

$\int \frac{1}{x} dx = ln(|x|) + C$

$\int \frac{1}{\sqrt{a^2-x^2}} dx = arcsin(\frac{x}{a}) + C$

$\int \frac{1}{a^2 + x^2} dx = \frac{1}{a}arctan(\frac{x}{a}) + C$

### Options for integration

U-substition, completing the square + trig, integration by parts, partial fraction


## Unit 7: Applications of differentiation

Slope fields: A graphical representation of solutions to a differential equation.

Euler's method: An approximation method for finding a solution to a differential equation.

Separable differential equation: A differential equation that can be written in the form $f(x) \, dx = g(y) \, dy$.

Logistic equation: $\frac{dN}{dt} = kN\left(1 - \frac{N}{c}\right)$, where $c$ is the carrying capacity and $k$ is the proportionality constant.


## Unit 8: Applications of integration

Average value of a function: area of function / length of range

Disk / Washer method: for finding volume by rotation

Arc length: take hypotenuses of many little right triangles of width dx and height dy, get $\int \sqrt{1+(\frac{dy}{dx})^2}dx$


## Unit 9: Parametric equations, polar coordinates, and vector-valued functions

Parametric equations: defining x and y in terms of a parameter

Represented as $\vec{r}(t) = \langle x(t), y(t) \rangle$.

## Unit 10: Infinite sequences and series

### Divergence and Convergence Tests

n-th term test: If $a_n$ does not converge to $0$, then the series $\sum a_n$ definitely diverges.

Integral test: For a positive, continuous, and decreasing function $f(x)$, the improper integral $\int_1^\infty f(x) \, dx$ can be used to estimate the area of the series. The behaviour of the series is the same as that of the integral.

p-series: A series of the form $\sum \frac{1}{n^p}$ converges if and only if $p > 1$.

Comparison test: Compare $\sum a_n$ to another series $\sum b_n$ where $b_n$ is known. If $0 \leq a_n \leq b_n$ for all $n$, then:
- If $\sum b_n$ converges, so does $\sum a_n$.
- If $\sum a_n$ diverges, so does $\sum b_n$.

Limit comparison test: For $\sum a_n$ and $\sum b_n$ with $a_n, b_n > 0$, if $\lim_{n \to \infty} \frac{a_n}{b_n} = c$, where $c > 0$ is finite, then both series converge or diverge together.

Alternating series test: For an alternating series $\sum (-1)^n b_n$, where $b_n$ is positive:
- If $b_n$ is decreasing and $\lim_{n \to \infty} b_n = 0$, then the series converges.
- This test does not provide information about divergence.

Ratio test: Consider the ratio $\lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right|$:
- If the ratio is $< 1$, the series converges absolutely.
- If the ratio is $> 1$, the series diverges.
- If the ratio is $= 1$, the test is inconclusive.

Conditional and absolute convergence:
- A series $\sum a_n$ converges absolutely if $\sum |a_n|$ converges.
- A series converges conditionally if $\sum a_n$ converges but $\sum |a_n|$ diverges.


### Approximating functions with polynomials

McLaurin series: Taylor series centered at 0

Taylor series: $P(x) = \sum^{\infty}_{n=0}\frac{1}{n!}f^{(n)}(a) * (x-a)^n$, where the polynomial is centered around a.

An geometric sum can be converted back to an infinite series if it's in the approrpiate form.

function -> geo series
series -> function

interval of convergence (radius is half the interval), make sure to check endpoints

match the constant

basically find a power series to approximate function

The Maclaurin series expansions for the common functions are:

$$\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \dots$$
$$\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \dots$$
$$e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \frac{x^4}{4!} + \dots$$
