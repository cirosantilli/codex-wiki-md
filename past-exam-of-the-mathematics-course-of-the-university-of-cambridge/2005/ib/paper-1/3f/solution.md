<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) states that if $f$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on a neighborhood of a positively oriented simple closed contour $C$ and its interior, then for $w$ inside,

$$
f(w)=\frac1{2\pi i}\int_C\frac{f(z)}{z-w}\,dz.
$$

For the given counterclockwise circle, divide the rational function:

$$
\frac{z^3}{z^2+1}=z-\frac12\left(\frac1{z-i}+\frac1{z+i}\right).
$$

The [contour integral](../../../../../contour-integral.md) of $z$ is zero because it has a primitive, while both points $\pm i$ lie inside the circle. Applying the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) to the constant function $1$ at each point gives

$$
\boxed{\int_{|z|=2}\frac{z^3}{z^2+1}\,dz=-2\pi i}.
$$

The sign reverses if the contour orientation is reversed.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
