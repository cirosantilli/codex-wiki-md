<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For general $\alpha>0$, put $S(\lambda)=\lambda^{-4}+2\lambda^2$. The reduced [strain energy density](../../../../../strain-energy-density.md) and its derivative are

$$
h(\lambda)=\frac\mu2\left[S(\lambda)^\alpha-3^\alpha\right],\qquad
h'(\lambda)=2\mu\alpha S(\lambda)^{\alpha-1}(\lambda-\lambda^{-5}).
$$

The same factorization as in part (i) yields

$$
\frac{h'(\lambda)}{\lambda^3-1}
=2\mu\alpha S(\lambda)^{\alpha-1}
\left(\lambda^{-2}+\lambda^{-5}\right).
$$

This form removes the apparent singularity at $\lambda=1$: its limit is $4\mu\alpha3^{\alpha-1}$, finite for every fixed $\alpha>0$. Thus only the upper endpoint can obstruct convergence of the [improper integral](../../../../../improper-integral.md).

As $\lambda\to\infty$, $S(\lambda)\sim2\lambda^2$, giving

$$
\frac{h'(\lambda)}{\lambda^3-1}
\sim\mu\alpha2^\alpha\lambda^{2\alpha-4}.
$$

For $\mu>0$, the [comparison test](../../../../../direct-comparison-test.md) with a power [integral](../../../../../integral-split.md) implies convergence exactly when $2\alpha-4<-1$. Therefore

$$
\boxed{0<\alpha<\frac32}
$$

is precisely the range with finite critical [pressure](../../../../../pressure-split.md), the [cavitation criterion for power-law strain energy](../../../../../cavitation-criterion-for-power-law-strain-energy.md). At $\alpha=3/2$ the divergence is logarithmic; for larger $\alpha$ it is a power divergence. These materials require an unbounded tensile loading magnitude in this ideal model. The qualification $\mu>0$ excludes the degenerate zero-energy material.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the solid mechanics course of the University of Oxford](../../../../split.md)
6. [Solid mechanics course of the University of Oxford](../../../../../solid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
