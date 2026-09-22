<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The side of the inscribed [equilateral triangle](../../../../../equilateral-triangle.md) has length $\sqrt3\,r$. If $d$ is the distance of a [chord](../../../../../chord-of-a-circle.md) midpoint from the center, a right triangle gives [chord](../../../../../chord-of-a-circle.md) length $2\sqrt{r^2-d^2}$. Thus a [chord](../../../../../chord-of-a-circle.md) is sufficiently long exactly when $d<r/2$.

**(a)** Uniform midpoint area puts the midpoint in the radius-$r/2$ [disk](../../../../../disk-mathematics.md) with [probability](../../../../../probability.md)

$$
\boxed{\frac{\pi(r/2)^2}{\pi r^2}=\frac14.}
$$

**(b)** Fix the first endpoint by rotational symmetry. [Independence](../../../../../independent-random-variables.md) and uniformity make the angle $\theta$ of the second endpoint uniform on $[0,2\pi)$. Its [chord](../../../../../chord-of-a-circle.md) length is $2r\sin(\theta/2)$, so the required event is $2\pi/3<\theta<4\pi/3$. Hence

$$
\boxed{\frac{4\pi/3-2\pi/3}{2\pi}=\frac13.}
$$

**(c)** If the midpoint distance itself has [uniform distribution](../../../../../continuous-uniform-distribution.md) on $[0,r]$, the event $d<r/2$ has [probability](../../../../../probability.md)

$$
\boxed{\frac12.}
$$

These are three different [probability measures](../../../../../probability-measure.md) on [chords](../../../../../chord-of-a-circle.md). Their different answers are [Bertrand's paradox](../../../../../bertrand-paradox-probability.md): specifying what is uniform is indispensable. Uniform area, uniform endpoints and uniform radial distance are not interchangeable sampling rules. Equality at the length threshold has [probability](../../../../../probability.md) zero in all three models.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
