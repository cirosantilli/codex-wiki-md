<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

For a regular curve, the [curvature and torsion](../../../../../curvature-and-torsion.md) definition gives

$$
\kappa=\left|\frac{dT}{ds}\right|
+=\frac{|\gamma'\times\gamma''|}{|\gamma'|^3}.
$$

It measures the rate at which the unit tangent turns per unit arclength.

Here

$$
\gamma'(t)=(-2\sin2t,\sqrt5,2\cos2t),
\qquad
\gamma''(t)=(-4\cos2t,0,-4\sin2t).
$$

Thus $|\gamma'|=3$, $|\gamma''|=4$, and $\gamma'\cdot\gamma''=0$. Hence

$$
|\gamma'\times\gamma''|=|\gamma'||\gamma''|=12,
\qquad
\boxed{\kappa=\frac{12}{27}=\frac49}.
$$

The [arc-length parametrization](../../../../../arc-length-parametrization.md) from $t=0$ is $s=3t$, so the curvature remains the constant $\kappa(s)=4/9$ for $0\leq s\leq3\pi$. Therefore the [total curvature](../../../../../total-curvature.md) is

$$
\boxed{\int_\gamma\kappa\,ds
+=\frac49(3\pi)=\frac{4\pi}{3}}.
$$

The curve $\widetilde\gamma$ is a unit circle traversed once. Its curvature is one and its length is $2\pi$, so without further calculation

$$
\boxed{\int_{\widetilde\gamma}\kappa\,ds=2\pi}.
$$

The helical curve $\gamma$ devotes part of its unit tangent to the constant vertical direction. Its tangent therefore turns more slowly on the unit sphere than the tangent to the planar circle, which explains the smaller total curvature.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
