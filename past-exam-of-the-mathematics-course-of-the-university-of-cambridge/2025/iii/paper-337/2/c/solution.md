<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\xi=v_F(k)\ell$ and use the same $\nu_F$. With a symmetric cutoff $|\xi|<\Lambda$, the [BCS gap equation](../../../../../../bcs-gap-equation.md) becomes

$$
\frac1{|V|}
=\nu_F\int_{-\Lambda}^{\Lambda}d\xi
\int_{-\infty}^{\infty}\frac{d\omega}{2\pi}
\frac1{\omega^2+\xi^2+\Delta^2}.
$$

The frequency integral is $1/[2\sqrt{\xi^2+\Delta^2}]$, so

$$
\frac1{\nu_F|V|}
=\operatorname{arsinh}\frac\Lambda\Delta
\sim\log\frac{2\Lambda}{\Delta}
\qquad(\Delta\ll\Lambda).
$$

Thus

$$
\boxed{
\Delta\sim2\Lambda
\exp\left[-\frac1{\nu_F|V|}\right].}
$$

The gap and the one-loop strong-coupling scale have the same nonperturbative exponential dependence; their order-one prefactors depend on the cutoff convention and microscopic completion. The renormalization-group divergence is therefore the normal-state signal of the paired, gapped phase found from the self-consistent gap equation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
