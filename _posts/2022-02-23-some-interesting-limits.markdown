---
title:  "Some interesting limits"
date:   2022-02-23 12:10:00 +0100
categories: math
---
<h2>$$\lim_{x \to 0^+} x \cdot ln(x)$$</h2>

Let's find the limit of $x \cdot ln(x)$, as $x \rightarrow 0$ from the right. In other words $\displaystyle{\lim_{x \to 0^+}} x \cdot ln(x)$.

A left sided limit is not defined, because when $x \rightarrow 0$ from the left, the ln function is undefined.

By substituting $t$ for $\frac{1}{x}$, we can instead find the limit as t approaches infinity.

$\displaystyle{t=\frac{1}{x}}$

$\displaystyle{\lim_{t \to \infty}}\frac{1}{t} \cdot \ln\frac{1}{t}$

We simplify the expression. Normal logarithm laws apply since we know that $t > 0$.

$\displaystyle{\ln\frac{1}{t}=\ln 1 - \ln t = -\ln t}$

$\displaystyle{\lim_{t \to \infty}}\frac{1}{t} \cdot (-\ln t) = -\lim_{t \to \infty}\frac{\ln t}{t}$

We know that a power, such as $t^1$, grows faster than a logarithm.

$\displaystyle{-\lim_{t \to \infty}}\frac{\ln t}{t} = -0 = 0$

<h2>$$\lim_{x \to 0} \frac{sin(x)}{x}$$</h2>
