<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [Green function of killed planar Brownian motion](../../../../../../green-function-of-killed-planar-brownian-motion.md), normalized as the density of expected occupation with respect to area:

$$
\mathbb E_z\int_0^T f(B_t)\,dt
=\int_D G_D(z,w)f(w)\,dA(w)
$$

for nonnegative measurable $f$. Equivalently, $G_D(z,w)=\int_0^\infty p_D(t,z,w)\,dt$, where $p_D$ is the [killed Brownian transition density](../../../../../../killed-brownian-transition-density.md). With generator $\tfrac12\Delta$, the distributional normalization is $-\tfrac12\Delta_wG_D(z,w)=\delta_z(w)$, and the singularity is $-\pi^{-1}\log|w-z|$ plus a locally [harmonic function](../../../../../../harmonic-function.md). This fixes the normalization of the [Dirichlet Green function](../../../../../../dirichlet-green-function.md) explicitly.

By [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md) and its [conformal Brownian clock](../../../../../../conformal-brownian-clock.md),

$$
\mathbb E_{z'}\int_0^{T'} f(B'_s)\,ds
=\mathbb E_z\int_0^T f(\phi(B_t))|\phi'(B_t)|^2\,dt
=\int_D G_D(z,w)f(\phi(w))|\phi'(w)|^2\,dA(w).
$$

The [Jacobian determinant](../../../../../../jacobian-determinant.md) of a [conformal map](../../../../../../conformal-map.md) is $|\phi'(w)|^2$. Changing the area variable to $w'=\phi(w)$ gives

$$
\int_{D'}G_D(z,\phi^{-1}(w'))f(w')\,dA(w').
$$

Uniqueness of the occupation density proves the desired equality almost everywhere. Both functions are continuous and [harmonic](../../../../../../harmonic-function.md) away from their pole, so it holds at every $w\ne z$. **The Green function is conformally invariant**:

$$
\boxed{G_{D'}(\phi(z),\phi(w))=G_D(z,w).}
$$

If the [Dirichlet Green function](../../../../../../dirichlet-green-function.md) is instead normalized for $-\Delta$, both kernels are divided by two and the invariance statement is unchanged.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
