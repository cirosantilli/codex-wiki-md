<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume sufficient decay and [differentiability](../../../../../differentiability.md) to justify [integration by parts](../../../../../integration-by-parts.md) and exchange of [integrals](../../../../../integral-split.md); [Schwartz functions](../../../../../schwartz-function.md) are one convenient class. With the stated [Fourier transform](../../../../../fourier-transform-split.md) convention, integrate first in $x$:

$$
\begin{aligned}
\mathcal F[u_x]
&=\int_{\mathbb R}e^{-ik_yy}\left([u e^{-ik_xx}]_{-\infty}^{\infty}+ik_x\int_{\mathbb R}u e^{-ik_xx}\,dx\right)dy\\
&=\boxed{ik_x\widehat u}.
\end{aligned}
$$

The boundary contribution vanishes under the decay assumption. The [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) consequently turns constant-coefficient spatial [differential operators](../../../../../differential-operator.md) into multipliers. Repeating it gives $\mathcal F[u_{xx}]=-k_x^2\widehat u$, so the [heat equation](../../../../../heat-equation.md) becomes an independent temporal [ordinary differential equation](../../../../../ordinary-differential-equation.md) at each [wavevector](../../../../../wavevector.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2025](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
