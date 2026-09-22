<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the nonpolynomial [function](../../../../../function-split.md) $f(x)=1+\sin x$ on $[-1,1]$. Its exact [integral](../../../../../integral-split.md) is

$$
\int_{-1}^1(1+\sin x)\,dx=2,
$$

because the [sine](../../../../../sine.md) is an [odd function](../../../../../odd-function.md).

For every uniform [partition of an interval](../../../../../partition-of-an-interval.md) with $N\geq1$ panels, the [quadrature nodes](../../../../../quadrature-node.md) satisfy $x_{N-j}=-x_j$. Their [composite trapezoidal rule](../../../../../composite-trapezoidal-rule.md) [quadrature weights](../../../../../quadrature-weight.md) agree, so the two sampled sine values cancel. If there is a node at zero its sine value is already zero. The constant term is integrated exactly, giving

$$
\boxed{T_N(1+\sin x)=2\quad\text{for every }N\geq1.}
$$

This is [symmetric trapezoidal exactness for odd functions](../../../../../symmetric-trapezoidal-exactness-for-odd-functions.md), applied after adding a [constant function](../../../../../constant-function.md) so that the resulting [definite integral](../../../../../definite-integral.md) is nonzero. It is exactness for this particular [integrand](../../../../../integrand.md), rather than a claim that every nonpolynomial [function](../../../../../function-split.md) is integrated exactly.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
