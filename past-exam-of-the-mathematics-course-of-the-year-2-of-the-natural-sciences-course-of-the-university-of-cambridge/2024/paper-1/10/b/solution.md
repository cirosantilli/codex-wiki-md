<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Sturm-Liouville eigenfunction expansion](../../../../../sturm-liouville-eigenfunction-expansion.md) of a suitable real function $f$ is

$$
f(x)=\sum_ny_n(x)\int_a^bw(\xi)y_n(\xi)f(\xi)\,d\xi=\int_a^b\left[w(\xi)\sum_ny_n(\xi)y_n(x)\right]f(\xi)\,d\xi.
$$

Comparing this identity with the sampling property of the [Dirac delta distribution](../../../../../dirac-delta-function.md) gives the completeness kernel

$$
\boxed{w(\xi)\sum_ny_n(\xi)y_n(x)=\delta(x-\xi).}
$$

This is an identity of [distributions](../../../../../distribution-mathematical-analysis.md), rather than a pointwise-convergent series of ordinary functions.

Assuming zero is not an [eigenvalue](../../../../../eigenvalue.md), define the [spectral Green function of a regular Sturm-Liouville problem](../../../../../spectral-green-function-of-a-regular-sturm-liouville-problem.md) by

$$
\boxed{G(x;\xi)=\sum_n\frac{y_n(x)y_n(\xi)}{\lambda_n}.}
$$

Applying $\mathcal L_x$ gives $w(x)\sum_ny_n(x)y_n(\xi)=\delta(x-\xi)$: multiplying the preceding completeness kernel by $w(x)/w(\xi)$ leaves the [Dirac delta distribution](../../../../../dirac-delta-function.md) unchanged. Each term also obeys the same homogeneous [boundary conditions](../../../../../boundary-condition.md). There is no extra weight factor in $G$ for the ordinary source measure $d\xi$.

If zero is an [eigenvalue](../../../../../eigenvalue.md), the inverse [Green's function](../../../../../green-s-function-split.md) does not exist on all forcing functions: the forcing must obey the [solvability condition at a Sturm-Liouville eigenvalue](../../../../../solvability-condition-at-a-sturm-liouville-eigenvalue.md). Omitting the zero mode instead constructs a reduced inverse, with its projection removed from the right-hand side. This exception occurs in part (c) at $\alpha=1$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
