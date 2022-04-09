---
title:  "The limit of sinx over x"
date:   2022-03-04 20:28:00 +0100
categories: math
---
vad är int(lnx)?
visa tricket med int(lnx) = int(1*lnx) med partiell integration blir det xlnx - x
visa att det går även för typ int(ln(x + 3))

<h2>$$\lim_{x \to 0} \frac{\sin(x)}{x} = 1$$</h2>

Here we will prove that $\displaystyle{\lim_{x \to 0} \frac{\sin(x)}{x} = 1}$.

<img src="/images/limit_sinx_over_x.png"/>

In the picture above we see a geometrical representation of sin and tan on the unit circle.

Let $0 < x < \frac{\pi}{2}$.

From the picture we can see three things:
1. The area of the triangle $\triangle ABC$ is $\frac{1}{2} \cdot \sin(x)$, since the height of the triangle is $\sin(x)$ and the base is $1$.
2. The area of the circle sector $ABC$ is $\frac{1}{2} \cdot x$.
3. The area of the triangle $\triangle ABD$ is $\frac{1}{2} \cdot \tan(x)$.

We can see that

$\frac{1}{2} \sin(x) \leq \frac{1}{2} x \leq \frac{1}{2} \tan(x)$.

If we divide by $\frac{1}{2}sin(x)$, which is a positive number since $0 < x < \frac{\pi}{2}$, we get

$1 \leq \frac{x}{\sin(x)} \leq \frac{1}{\cos(x)}$.

We then take the reciprocals, and in the process reversing the inequalities

$\frac{1}{1} \geq \frac{1}{\frac{x}{\sin(x)}} \geq \frac{1}{\frac{1}{\cos(x)}} =$

$1 \geq \frac{\sin(x)}{x} \geq \cos(x)$.

Now, since $\displaystyle{\lim_{x \to 0} \cos(x) = 1}$, the Squeeze Theorem tells us that

$\displaystyle{\lim_{x \to 0} \frac{\sin(x)}{x} = 1}$.
