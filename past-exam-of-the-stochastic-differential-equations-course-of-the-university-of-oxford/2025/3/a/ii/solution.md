<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [Itô formula](../../../../../ito-s-lemma.md) to $M_t=e^{X_t}$. Since $d[X]_t=\sigma(X_t)^2dt$ and $b=-\sigma^2/2$, the two [drift](../../../../../drift-coefficient.md) terms cancel:

$$
dM_t=e^{X_t}dX_t+\frac12e^{X_t}d[X]_t
=\frac{e^{X_t}}{1+X_t^2}\,dB_t.
$$

The integrand is continuous and hence locally square integrable after stopping at bounded levels of $X$. Thus $M$ is a positive [continuous local martingale](../../../../../continuous-local-martingale.md), with $M_0=1$ and [quadratic variation](../../../../../quadratic-variation.md)

$$
\boxed{M_t=1+\int_0^t\frac{e^{X_s}}{1+X_s^2}\,dB_s,\qquad
[M]_t=\langle M\rangle_t=\int_0^t\frac{e^{2X_s}}{(1+X_s^2)^2}\,ds.}
$$

The cancellation is the reason $e^x$ is the relevant [scale function](../../../../../scale-function-stochastic-processes.md) for this diffusion.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
