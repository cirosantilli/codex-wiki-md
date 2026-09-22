<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under $H_0$, each $Z_i=-\log X_i$ has [expected value](../../../../expected-value-split.md) $1/2$ and [variance](../../../../variance-split.md) $1/4$. The [central limit theorem](../../../../central-limit-theorem.md) therefore approximates

$$
\frac{S-n/2}{\sqrt n/2}\ \mathrel{\dot\sim}\ N(0,1).
$$

For the supplied data this standardized value is

$$
\boxed{z_{\mathrm{obs}}=\frac{6.25-12.5}{2.5}=-2.5}.
$$

Using the provided approximation $\Phi(1.6)\approx0.95$, the lower-tail 5% rule rejects when $S\leq12.5-1.6(2.5)=8.5$. The observed $6.25$ is in this region, with approximate [p-value](../../../../p-value.md) $\Phi(-2.5)\approx0.005$. **Reject $H_0:\theta=2$ at the 5% level in favor of the specified alternative $\theta=3$.** The unusually large [geometric mean](../../../../geometric-mean.md) is consistent with the direction of that alternative. This is evidence in this comparison, not a proof that the parameter is exactly three.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
