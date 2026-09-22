<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $g_K(iy)=u_y+iv_y$. The [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md) gives

$$
u_y=O(y^{-2}),\qquad v_y=y-\frac{a_K}{y}+O(y^{-2}),
\qquad \frac{v_y}{y}\to1.
$$

The real interval under consideration lies outside the hull, so the reflected boundary map sends it monotonically to $(g_K(x),g_K(b))$. [Conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md) transports its [harmonic measure](../../../../../../harmonic-measure.md) to the half-plane. By the [Poisson kernel for the upper half-plane](../../../../../../poisson-kernel-for-the-upper-half-plane.md),

$$
\mathbb P_{iy}(B_T\in(x,b))
=\frac1\pi\int_{g_K(x)}^{g_K(b)}
\frac{v_y}{(r-u_y)^2+v_y^2}\,dr.
$$

The endpoints are fixed and finite. On this interval,

$$
\frac{y v_y}{(r-u_y)^2+v_y^2}\longrightarrow1
$$

uniformly, using $v_y/y\to1$ and $u_y\to0$. Integrating gives **the interval-length limit**:

$$
\boxed{\lim_{y\to\infty}\pi y\,\mathbb P_{iy}(B_T\in(x,b))
=g_K(b)-g_K(x).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
