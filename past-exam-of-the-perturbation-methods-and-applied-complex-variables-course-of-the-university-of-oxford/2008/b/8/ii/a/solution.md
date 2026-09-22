<h1 id="b/8/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\operatorname{Im}k>0$, put $s=-ik$, so $\operatorname{Re}s>0$. The [Laplace transform](../../../../../../laplace-transform.md) for the [Gamma function](../../../../../../gamma-function.md), analytically continued from positive real $s$, gives

$$
\int_0^\infty x^{-1/4}e^{ikx}\,dx
=\Gamma(3/4)(-ik)^{-3/4}.
$$

Choose $\arg k\in(0,\pi)$ in the [upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). Since $\arg(-ik)=\arg k-\pi/2$,

$$
\boxed{\int_0^\infty x^{-1/4}e^{ikx}\,dx
=\Gamma(3/4)e^{3i\pi/8}k^{-3/4}.}
$$

This integral is absolutely convergent throughout the [upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). On the nonzero [real axis](../../../../../../real-axis.md) it converges conditionally by [Dirichlet test for improper integrals](../../../../../../dirichlet-test-for-improper-integrals.md), and its value is the upper boundary limit of the same branch. In particular negative real $k$ has argument $\pi$, not $-\pi$ in this formula.

At $k=0$ the integral diverges at infinity; in the lower [half-plane](../../../../../../half-plane.md) its [exponential function](../../../../../../exponential-function.md) factor grows and the ordinary improper integral diverges. The origin itself causes no local-integrability problem for $x^{-1/4}$. A useful continuation of the chosen power uses a [branch cut](../../../../../../branch-cut.md) descending from $k=0$ with argument in $(-\pi/2,3\pi/2)$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [8](../../../8.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../../split.md)
7. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
