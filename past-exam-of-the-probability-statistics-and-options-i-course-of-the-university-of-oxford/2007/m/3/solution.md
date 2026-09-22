<h1 id="m/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [moment-generating function](../../../../moment-generating-function.md) is $M_X(t)=\mathbb E e^{tX}$ on the real values where this expectation is finite, normally including a neighborhood of zero. Direct substitution gives

$$
\boxed{M_{aX+b}(t)=e^{bt}M_X(at)}
$$

whenever the right side is finite.

For the given [Gamma distribution](../../../../gamma-distribution.md) and $t<\lambda$,

$$
M_X(t)=\frac{\lambda^m}{(m-1)!}
\int_0^\infty x^{m-1}e^{-(\lambda-t)x}dx
=\left(\frac\lambda{\lambda-t}\right)^m,
$$

using the [Gamma function](../../../../gamma-function.md) after the scaling $u=(\lambda-t)x$. At $t\geq\lambda$ the positive integral diverges.

[independence](../../../../independent-random-variables.md) multiplies [moment-generating functions](../../../../moment-generating-function.md). Thus

$$
M_{\sum_iY_i}(t)=\left(\frac\lambda{\lambda-t}\right)^{2n}.
$$

Uniqueness of a [moment-generating function](../../../../moment-generating-function.md) on a neighborhood of zero identifies

$$
\boxed{\sum_{i=1}^nY_i\sim\operatorname{Gamma}(2n,\lambda),}
$$

where $\lambda$ is the rate parameter, as in the printed [probability density function](../../../../probability-density-function.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [M](../../m.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
