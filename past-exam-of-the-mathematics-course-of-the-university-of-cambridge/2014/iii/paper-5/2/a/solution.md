<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The total differential order of $\partial_t-\partial_x^2$ is two, so its [principal symbol](../../../../../../principal-symbol-of-a-partial-differential-equation.md) is $p(\tau,\xi)=-\xi^2$. The conormal to $t=0$ is $(1,0)$, on which $p$ vanishes. **The initial line is a [characteristic hypersurface](../../../../../../characteristic-hypersurface.md)** for this total-order symbol; the first-order time derivative does not enter it.

Suppose a [real analytic](../../../../../../real-analytic-function.md) solution existed near $(0,0)$. Repeated use of the [heat equation](../../../../../../heat-equation.md) gives $\partial_t^k u=\partial_x^{2k}u$. The initial [power series](../../../../../../power-series.md) is $\sum_{j\geq0}(-1)^j x^{2j}$ near zero, hence

$$
\partial_t^k u(0,0)=(-1)^k(2k)!.
$$

The time [Taylor series](../../../../../../taylor-series.md) at $x=0$ would therefore have coefficients $(-1)^k(2k)!/k!$. The ratio of successive absolute coefficients is $2(2k+1)\to\infty$, giving radius of convergence zero. This contradicts the assumed [real analytic](../../../../../../real-analytic-function.md) regularity. **No such analytic local solution exists**, although the initial function itself is [real analytic](../../../../../../real-analytic-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
