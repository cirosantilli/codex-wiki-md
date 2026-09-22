<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

A [smooth surface](../../../../../smooth-surface.md) in $\mathbb R^3$ is a subset locally parametrized by a smooth map of two variables whose derivative has rank two and which is a homeomorphism onto its image.

Writing $\rho=\sqrt{x^2+y^2}$, the first surface equation becomes

$$
(\rho-2\sqrt2)^2+z^2=1.
$$

It is the [torus](../../../../../torus.md) of major radius $R=2\sqrt2$ and minor radius $r=1$, with smooth parametrization

$$
\boxed{X(u,v)=((2\sqrt2+\cos v)\cos u,
(2\sqrt2+\cos v)\sin u,\sin v)},
\qquad u,v\in\mathbb R/(2\pi\mathbb Z).
$$

Since $R>r$, this is an embedding. The [Gaussian curvature of a torus](../../../../../gaussian-curvature-of-a-torus.md) is

$$
\boxed{K(u,v)=\frac{\cos v}{2\sqrt2+\cos v}}.
$$

For the second surface, use the [orthogonal transformation](../../../../../orthogonal-transformation.md)

$$
X=\frac{x+z}{\sqrt2},
\qquad Y=y,
\qquad Z=\frac{z-x}{\sqrt2}.
$$

Its equation becomes the same torus equation $(\sqrt{X^2+Y^2}-2\sqrt2)^2+Z^2=1$. Orthogonal transformations are Euclidean [isometries](../../../../../isometry.md) and preserve [Gaussian curvature](../../../../../gaussian-curvature.md). Curvature vanishes where $\cos v=0$, equivalently $Z=\pm1$. In the original coordinates the zero-curvature points are therefore exactly

$$
\boxed{z-x=\pm\sqrt2,
\qquad (x+z)^2+2y^2=16}.
$$

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
