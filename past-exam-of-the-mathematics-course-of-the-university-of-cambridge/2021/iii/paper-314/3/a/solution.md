<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $\nabla\phi=\mathbf e_\phi/r$, the vector field has cylindrical components

$$
\mathbf A=-\frac{\alpha_z}{r}\mathbf e_r
+\frac\beta r\mathbf e_\phi
+\frac{\alpha_r}{r}\mathbf e_z.
$$

The [divergence](../../../../../../divergence.md) in cylindrical coordinates is therefore

$$
\nabla\cdot\mathbf A
=-\frac1r\partial_r\alpha_z
+\frac1r\partial_z\alpha_r=0.
$$

Direct use of the [curl](../../../../../../curl.md) in cylindrical coordinates gives

$$
(\nabla\times\mathbf A)_r=-\frac{\beta_z}{r},
\qquad
(\nabla\times\mathbf A)_z=\frac{\beta_r}{r},
$$

and

$$
(\nabla\times\mathbf A)_\phi
=\frac1r\left[-r\partial_r(r^{-1}\alpha_r)-\alpha_{zz}\right].
$$

Thus, defining

$$
\boxed{L\alpha=-r\partial_r(r^{-1}\partial_r\alpha)-\partial_z^2\alpha},
$$

we obtain

$$
\boxed{\nabla\times\mathbf A
=\nabla\beta\times\nabla\phi+(L\alpha)\nabla\phi}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
