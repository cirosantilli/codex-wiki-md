<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $F(z)=z+z^{-1}$. On the unit semicircle, $F(e^{i\theta})=2\cos\theta$, and

$$
\left|\frac d{d\theta}F(e^{i\theta})\right|=2\sin\theta.
$$

The [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md) and the [Poisson kernel for the upper half-plane](../../../../../../poisson-kernel-for-the-upper-half-plane.md) therefore give the exit density with respect to $d\theta$:

$$
p(z,e^{i\theta})
=\frac1\pi
\frac{\operatorname{Im}F(z)}
{|F(z)-2\cos\theta|^2}\,2\sin\theta.
$$

As $z\to\infty$ in $\mathbb H$,

$$
\operatorname{Im}F(z)
=\operatorname{Im}z\left(1-\frac1{|z|^2}\right),
\qquad
|F(z)-2\cos\theta|^2
=|z|^2\bigl(1+O(|z|^{-1})\bigr),
$$

uniformly in $\theta\in[0,\pi]$. Hence

$$
\boxed{p(z,e^{i\theta})
=\frac2\pi\frac{\operatorname{Im}z}{|z|^2}
\sin\theta\bigl(1+O(|z|^{-1})\bigr).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
