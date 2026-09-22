<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Minimize or maximize $D(x)=x^Tx$ subject to $x^TAx=1$. A [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\Lambda$ gives

$$
2x-2\Lambda Ax=0.
$$

The constraint excludes $x=0$ and implies $Ax\neq0$, so it is a regular constraint surface. Multiplying the stationarity equation by $x^T$ gives $D=\Lambda>0$. Thus the [distance extrema on a real quadratic surface](../../../../../distance-extrema-on-a-real-quadratic-surface.md) satisfy

$$
\boxed{Ax=\frac1D x.}
$$

Every constrained extremum lies in a positive-eigenvalue [eigenspace](../../../../../eigenspace.md), with squared distance $D=1/\lambda$. If $A$ is positive definite, the global minimum is $1/\lambda_{\max}$ and the global maximum is $1/\lambda_{\min}$. For an indefinite or singular form the surface need not be bounded; [eigenvector](../../../../../eigenvector.md) directions give stationary candidates, which may be saddles and need not supply both global extrema. With a repeated positive [eigenvalue](../../../../../eigenvalue.md), there can be an entire family of equally distant stationary points.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
