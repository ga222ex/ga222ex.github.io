---
title:  "Integrating 1 over x"
date:   2022-02-27 22:27:00 +0100
categories: math
---
<h2>$$\int \frac{1}{x}\;\mathrm{d}x$$</h2>

We want integrate $\frac{1}{x}$, which is the same as finding a primitive function of $\frac{1}{x}$.

From known differentiation rules we know that $\frac{d}{dx}\ln(x) = \frac{1}{x}$, which tells us that a primitive function for $\frac{1}{x}$ is $\ln(x) + C$. But there is a problem. The derivation rule we just applied is not defined for negative x. $\ln(x)$ is only defined for $x > 0$, while its derivative $\frac{1}{x}$ is defined for $x \neq 0$, so it is also defined for negative numbers. A derivative of a function can <strong>not</strong> be defined where the function is not. If a function is not defined somewhere, it cannot have a slope there. We need another approach.

Let us study the function $f(x) = \ln \lvert x \rvert$. The domain of that function is $x \neq 0$.

Let us further define $f(x) = \ln \lvert x \rvert$.

$\ln \lvert x \rvert = \ln(x)$ if $x > 0$ and
$\ln \lvert x \rvert = \ln(-x)$ if $x < 0$.

The minus sign before the x in $\ln(-x)$ might look scary, but remember that $-x > 0$ if $x < 0$.

Now let us differentiate these two functions individually.

$\frac{d}{dx}\ln(x) = \frac{1}{x}$ if $x > 0$

$\frac{d}{dx}\ln(-x) = \frac{1}{-x}\cdot (-1) = \frac{1}{x}$ if $x < 0$

In other words: $\frac{d}{dx}\ln \lvert x \rvert = \frac{1}{x}$ if $x \neq 0$

We can now safely say that $\int \frac{1}{x}\;\mathrm{d}x = \ln \lvert x \rvert + C$ if $x \neq 0$. The primitive function $\ln \lvert x \rvert + C$ is then defined for every x that $\frac{1}{x}$ is.
