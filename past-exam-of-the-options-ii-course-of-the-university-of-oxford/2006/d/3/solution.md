<h1 id="d/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [monotone convergence theorem](../../../../monotone-convergence-theorem.md) states that if $0\leq h_n\uparrow h$ pointwise almost everywhere and the functions are [measurable](../../../../measurability.md), then $\int h_n\uparrow\int h$, allowing the value infinity.

Interpret the displayed densities as zero outside $(0,1)$, so no undefined logarithm is evaluated there. Each $f_k$ is nonnegative and [measurable](../../../../measurability.md). With $x=e^{-t}$,

$$
\int_0^1-x^{2k}\log x\,dx
=\int_0^\infty t e^{-(2k+1)t}dt
=\boxed{\frac1{(2k+1)^2}},
$$

where the last equality is [integration by parts](../../../../integration-by-parts.md). This is finite, proving [Lebesgue integrability](../../../../integrability.md).

The nonnegative partial sums satisfy, for $0<x<1$,

$$
\sum_{k=0}^Nf_k(x)=-\log x\sum_{k=0}^Nx^{2k}
\ \uparrow\ -\frac{\log x}{1-x^2}=g(x).
$$

They vanish outside the interval as well. Monotone convergence therefore gives

$$
\boxed{\int_{\mathbb R}g(x)dx=\sum_{k=0}^\infty\frac1{(2k+1)^2}.}
$$

The series is finite by comparison with the convergent series $\sum_{j\geq1}j^{-2}$, whose convergence follows from the [integral test](../../../../integral-test-for-convergence.md). Since $g\geq0$, this finite integral proves absolute [Lebesgue integrability](../../../../integrability.md) as required.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [D](../../d.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
