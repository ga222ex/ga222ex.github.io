---
title:  "Some integrals"
date:   2022-04-09 14:45:00 +0100
categories: math calculus
---
<h2>$$\int sin^2xdx$$</h2>

Solving this intregal without modifying it first is difficult.

We can solve this integral using two different approaches. One where we simplify the expression using some well known trigonometric identities, and one where we use integration by parts. We begin with simplifying with trig formulas.

We know that $sin^2x + cos^2x = 1$. This is called the "Pythagorean trigonometric identity", or in swedish "Trigonometriska ettan". From that equation, we solve for $sin^2x$

$$sin^2x = 1 - cos^2x$$

Another trigonometric identity is $cos(2x) = cos^2x - sin^2x$, which we can rewrite as

$$cos(2x) = cos^2x - (1 - cos^2x) = 2 \cdot cos^2x - 1$$

Then we solve for $cos^2x$

$$\frac{cos(2x) + 1}{2} = cos^2x$$

Now we have something that is a bit easier to integrate

$$sin^2x = 1 - cos^2x = 1 - \frac{cos(2x) + 1}{2} = \frac{1}{2} - \frac{cos(2x)}{2}$$

$$\int (\frac{1}{2} - \frac{cos(2x)}{2})dx = \int \frac{1}{2}dx -\frac{1}{2} \int cos(2x)dx = \frac{x}{2} - \frac{sin(2x)}{4} + C$$

I will now show the method with integration by parts.

We want to solve $\int sin^2xdx$. $sin^2x$ can be written as $sin(x) \cdot sin(x)$. We now integrate by parts, where we differentiate one of the factors and integrate the other.

$$\int sin(x) \cdot sin(x) dx = -cos(x) \cdot sin(x) - \int -cos(x) \cdot cos(x) dx = -\frac{1}{2} \cdot 2 \cdot cos(x) \cdot sin(x) + \int cos^2(x)dx$$

By the double angle formula of sin, $2 sin(x) cos(x) = sin(2x)$ and by the Pythagorean trigonometric identity, $cos^2x = 1 - sin^2x$. So we can rewrite as

$$-\frac{1}{2} \cdot 2 \cdot cos(x) \cdot sin(x) + \int cos^2(x)dx = -\frac{1}{2} \cdot sin(2x) + \int (1 - sin^2x)dx = -\frac{1}{2} \cdot sin(2x) + \int 1dx -\int sin^2x)dx$$

So now we have

$$\int sin^2xdx = -\frac{1}{2} \cdot sin(2x) + \int 1dx -\int sin^2x)dx$$

$$\int sin^2xdx + \int sin^2x)dx= -\frac{1}{2} \cdot sin(2x) + \int 1dx$$

$$2 \cdot \int sin^2xdx = -\frac{1}{2} \cdot sin(2x) + x + C$$

$$\int sin^2xdx = -\frac{1}{4} \cdot sin(2x) + \frac{x}{2} + D$$
