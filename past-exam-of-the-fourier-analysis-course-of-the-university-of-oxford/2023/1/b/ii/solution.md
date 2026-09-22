<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $\alpha>1$, then $f_\alpha$ is an [integrable function](../../../../../lebesgue-integrable-function.md), so the [Riemann-Lebesgue lemma](../../../../../riemann-lebesgue-lemma.md) supplies a continuous representative of its [Fourier transform](../../../../../fourier-transform-split.md). Equivalently, in the mixture for $h_\alpha$ the majorant $t^{(\alpha-3)/2}e^{-t}$ is integrable at zero precisely when $\alpha>1$. In this case [dominated convergence](../../../../../dominated-convergence-theorem.md) also gives

$$
h_\alpha(0)=\frac{\sqrt\pi\,\Gamma((\alpha-1)/2)}{\Gamma(\alpha/2)}.
$$

If $0<\alpha\leq1$, [Fatou's lemma](../../../../../fatou-s-lemma.md) applied along any sequence of nonzero $\xi$ tending to zero gives

$$
\liminf_{\xi\to0,\,\xi\ne0}h_\alpha(\xi)
\geq\frac{\sqrt\pi}{\Gamma(\alpha/2)}\int_0^\infty t^{(\alpha-3)/2}e^{-t}\,dt=+\infty.
$$

The divergence comes from zero, where the exponent is at most $-1$. A continuous representative $H$ would agree with $h_\alpha$ [almost everywhere](../../../../../almost-everywhere.md). Since both are continuous on each open half-line, they must agree everywhere on those half-lines: a nonzero continuous difference would be nonzero on an interval of positive [Lebesgue measure](../../../../../lebesgue-measure.md). The displayed blow-up then contradicts continuity of $H$ at zero. Changing a value at one point cannot remove this singularity. Consequently

$$
\boxed{\widehat{f_\alpha}\text{ has a continuous representative on }\mathbb R\iff\alpha>1.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
