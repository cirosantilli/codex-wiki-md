<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under a country-specific [constant hazard survival model](../../../../../../../constant-hazard-survival-model.md), let $D_k$ be the number of deaths and $Y_k$ the total [person-time at risk](../../../../../../../person-time-at-risk.md) in country $k$. The likelihood is proportional to

$$
L_k(\lambda_k)\propto\lambda_k^{D_k}e^{-\lambda_kY_k},
$$

so the [maximum-likelihood estimator](../../../../../../../maximum-likelihood-estimator.md) is $\widehat\lambda_k=D_k/Y_k$. Test $H_0:\lambda_0=\lambda_1$ by a [likelihood-ratio test](../../../../../../../likelihood-ratio-test.md), [score test](../../../../../../../score-test.md), or [Wald test](../../../../../../../wald-test.md); equivalently, give $D_k$ a [Poisson distribution](../../../../../../../poisson-distribution.md) with mean $\lambda_kY_k$ and test the country coefficient in a [Poisson regression](../../../../../../../poisson-regression.md) with offset $\log Y_k$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
