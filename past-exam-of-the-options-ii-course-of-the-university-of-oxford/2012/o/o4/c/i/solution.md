<h1 id="o/o4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the shifted exponential model, $F(x)=1-e^{-\lambda(x-1)}$ for $x\geq1$. It is increasing, so the [probability integral transform](../../../../../../probability-integral-transform.md) preserves order: $F(X_{(r)})=Y_{(r)}$. The expected uniform plotting positions are $r/(n+1)$ by part (b). Replacing the random transformed [order statistic](../../../../../../order-statistic.md) by this representative position gives

$$
1-e^{-\lambda(x_{(r)}-1)}\approx\frac r{n+1},\qquad
x_{(r)}\approx1+\frac1\lambda\left[-\log\left(1-\frac r{n+1}\right)\right].
$$

Thus **plotting $x_{(r)}$ against $t_r=-\log(1-r/(n+1))$ should give an approximate [line](../../../../../../straight-line.md) with intercept one and slope $\boxed{1/\lambda}$**.

The replacement is a quantile-plot approximation, not an assertion that [expectation](../../../../../../expected-value-split.md) commutes exactly with the nonlinear inverse [distribution function](../../../../../../cumulative-distribution-function.md). The random points need not lie exactly on the [line](../../../../../../straight-line.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [O4](../../../o4.md)
4. [O](../../../../o.md)
5. [2012](../../../../../2012-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
