<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The null model's 99 residual [degrees of freedom](../../../../../../degree-of-freedom.md) imply $n=100$. Each predictor has a one-degree-of-freedom linear contribution in the parametric table, plus the reported nonlinear contribution. Consequently the termwise [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md) are

$$
\boxed{\mathrm{edf}_{\mathrm{experience}}\approx1+8.8=9.8,\qquad
\mathrm{edf}_{\mathrm{education}}\approx1+0.4=1.4.}
$$

Include the intercept once, giving **about $12.2$ total effective [degrees of freedom](../../../../../../degree-of-freedom.md)**. The more precise residual [degrees of freedom](../../../../../../degree-of-freedom.md) in the output give

$$
\boxed{\mathrm{edf}_{\mathrm{total}}=100-87.7644=12.2356.}
$$

There is no conflict: $8.8$ and $0.4$ are rounded, so they cannot recover the precise total. Individual unrounded termwise values are not provided.

The package's residual mean-square estimate of error [variance](../../../../../../variance-split.md) is

$$
\boxed{\widehat\sigma^2=\frac{906437.7}{87.7644}\approx10328.08,}
$$

matching the rounded $10328$ in the table. The nonlinear experience contribution is highly significant, while the smaller nonlinear education contribution has approximate $p=0.03923$.

This calculation uses the effective residual [degrees of freedom](../../../../../../degree-of-freedom.md) reported by this fit. For a general non-idempotent [linear smoother](../../../../../../linear-smoother.md) $S$, the noise contribution to expected RSS is $\sigma^2\operatorname{tr}[(I-S)^T(I-S)]$, and the expectation can additionally contain squared smoothing bias. Thus dividing by $n-\operatorname{tr}(S)$ is not a universal exact-unbiasedness theorem. The output's separation of linear and nonlinear term [degrees of freedom](../../../../../../degree-of-freedom.md) is documented at [https://cran.r-project.org/web/packages/gam/gam.pdf.](https://cran.r-project.org/web/packages/gam/gam.pdf.)

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
