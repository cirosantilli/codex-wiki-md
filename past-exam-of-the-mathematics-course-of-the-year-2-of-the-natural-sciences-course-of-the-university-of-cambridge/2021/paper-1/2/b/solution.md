<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For spherical symmetry the angular mode is $\ell=0$. Put $u(t,r)=r\psi(t,r)$. Direct differentiation gives

$$
\frac1{r^2}(r^2\psi_r)_r=\frac{u_{rr}}r,\qquad\psi_t=\frac{u_t}r,
$$

so the [radial heat equation in three dimensions](../../../../../radial-heat-equation-in-three-dimensions.md) becomes the ordinary one-dimensional [heat equation](../../../../../heat-equation.md) $u_t=\kappa u_{rr}$. Since $r_\pm>0$, the zero endpoint temperatures become $u(t,r_\pm)=0$.

Write $L=r_+-r_-$. The two initial sine modes already satisfy these [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md); their squared [wave numbers](../../../../../wavenumber.md) are $(\pi/L)^2$ and $(2\pi/L)^2$. Each therefore evolves independently with its corresponding [exponential decay](../../../../../exponential-decay.md). Dividing back by $r$ gives

$$
\boxed{\psi(t,r)=\frac1r\left[e^{-\kappa\pi^2t/L^2}\sin\frac{\pi(r_+-r)}L+e^{-4\kappa\pi^2t/L^2}\sin\frac{2\pi(r_+-r)}L\right].}
$$

At $t=0$ the initial profile is recovered, and each sine is zero at both endpoints. The first mode decays four times more slowly in its exponential rate than the second. This is the two-mode instance of the [spherical-shell heat equation via radial rescaling](../../../../../spherical-shell-heat-equation-via-radial-rescaling.md); uniqueness follows, for example, by applying the [heat equation energy identity](../../../../../heat-equation-energy-identity.md) to the difference of two solutions.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
