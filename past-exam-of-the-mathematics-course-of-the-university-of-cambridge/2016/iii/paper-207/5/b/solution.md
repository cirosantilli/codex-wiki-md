<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $U=H(T)$ and $V=H(C)$, so $Y=\min(U,V)$ and $0\le\mathbb EY\le\mathbb EU=1$. Its [expectation](../../../../../../expected-value.md) is not generally one and depends on censoring. Under [independent censoring](../../../../../../independent-censoring.md), condition on $V=v$: the [exponential distribution](../../../../../../exponential-distribution.md) gives

$$
\mathbb E(Y\mid V=v)=\int_0^v e^{-u}\,du=1-e^{-v}=\mathbb P(U\le V\mid V=v).
$$

Writing $\Delta=\mathbf1_{T\le C}$ for the observed event indicator, it follows that $\mathbb EY=\mathbb E\Delta$. The [exponential mean imputation under independent censoring](../../../../../../exponential-mean-imputation-under-independent-censoring.md) therefore gives **a [modified Cox–Snell residual](../../../../../../modified-cox-snell-residual.md) with known mean**:

$$
\boxed{Y^*=Y+(1-\Delta),\qquad\mathbb EY^*=1.}
$$

On censoring, the added one is the expected remaining transformed lifetime, by [memorylessness of the exponential distribution](../../../../../../memorylessness-of-the-exponential-distribution.md). This gives a mean-one variable, not necessarily another exponential variable. Equivalently, $M=\Delta-Y=1-Y^*$ is a [martingale residual](../../../../../../martingale-residual.md) with mean zero. [Independent censoring](../../../../../../independent-censoring.md), or its appropriate conditional version, is essential for these identities; arbitrary informative censoring does not justify the correction.

Fit a model using the relevant [covariates](../../../../../../covariate.md), calculate $\widehat M_i=v_i-\widehat H_i(x_i)$, and plot these [martingale residuals](../../../../../../martingale-residual.md) against a candidate explanatory variable or against an included variable's value. A smooth systematic trend away from zero can indicate an omitted effect or an unsuitable functional form, such as a nonlinear age effect. After fitting an appropriate effect, the residual trend should diminish. The equivalent plot of $\widehat Y_i^*$ has mean-one reference rather than zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
