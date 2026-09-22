<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Both kernels are [integrable functions](../../../../lebesgue-integrable-function.md), so the [convolution theorem](../../../../convolution-theorem.md) gives

$$
\widehat{q_t*q_s}(\omega)=\widehat q_t(\omega)\widehat q_s(\omega)
=e^{-(t+s)\omega^2}=\widehat q_{t+s}(\omega).
$$

The [uniqueness of the Fourier transform on integrable functions](../../../../uniqueness-of-the-fourier-transform-on-integrable-functions.md) gives equality almost everywhere. Both sides are continuous, so it holds at every point:

$$
\boxed{q_t*q_s=q_{t+s}.}
$$

For completeness, continuity of the convolution follows by [dominated convergence](../../../../dominated-convergence-theorem.md): $q_t$ is bounded and continuous, so for $x_j\to x$ the integrands $q_t(x_j-y)q_s(y)$ converge pointwise and are dominated by $\|q_t\|_\infty q_s(y)$.

The identity is the [heat semigroup](../../../../heat-semigroup.md) property: evolving for time $s$, then for time $t$, is the same as evolving once for time $s+t$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
