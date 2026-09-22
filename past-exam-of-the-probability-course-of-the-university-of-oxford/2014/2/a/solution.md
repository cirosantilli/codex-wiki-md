<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Integrating $e^{tx}$ against the [Gamma density](../../../../gamma-density.md) gives the [moment-generating function of a gamma distribution](../../../../moment-generating-function-of-a-gamma-distribution.md):

$$
M_X(t)=\frac{\lambda^r}{(r-1)!}\int_0^\infty x^{r-1}e^{-(\lambda-t)x}\,dx
=\boxed{\left(\frac{\lambda}{\lambda-t}\right)^r},\qquad t<\lambda.
$$

The [change of variables](../../../../change-of-variables-formula.md) $y=(\lambda-t)x$ reduces the integral to $\Gamma(r)=(r-1)!$ using the [gamma function](../../../../gamma-function.md). For $t\geq\lambda$ the defining integral is infinite. In particular the [moment-generating function](../../../../moment-generating-function.md) is finite on a [neighbourhood](../../../../neighbourhood-mathematics.md) of zero.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the probability course of the University of Oxford](../../../split.md)
5. [Probability course of the University of Oxford](../../../../probability-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
