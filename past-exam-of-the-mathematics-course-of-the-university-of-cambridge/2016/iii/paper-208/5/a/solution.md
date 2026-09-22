<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Y_i$ be iid with density $f$, set $H_i=h(Y_i)$, and put $I=E_fh(Y)$ and $\tau^2=\operatorname{Var}_f(h(Y))$. The finite-second-moment assumption gives, for $\tau^2>0$,

$$
\sqrt N(\widehat I_N-I)\Longrightarrow N(0,\tau^2),\qquad\widehat I_N=N^{-1}\sum_{i=1}^NH_i.
$$

The [sample variance](../../../../../../sample-variance.md) $s_N^2=(N-1)^{-1}\sum_i(H_i-\widehat I_N)^2$ consistently estimates $\tau^2$. The [central limit theorem](../../../../../../central-limit-theorem.md) and [Slutsky theorem](../../../../../../slutsky-theorem.md) therefore give the asymptotic [confidence interval](../../../../../../confidence-interval.md)

$$
\boxed{\left[\widehat I_N-z_{1-\alpha/2}\frac{s_N}{\sqrt N},\quad\widehat I_N+z_{1-\alpha/2}\frac{s_N}{\sqrt N}\right].}
$$

Its confidence probability is approximately $1-\alpha$, conventionally written $100(1-\alpha)\%$; the printed $(1-\alpha)\%$ omits the factor $100$. For $\tau^2=0$, $h(Y)=I$ almost surely and the estimator has zero error. This interval concerns iid [Monte Carlo estimators](../../../../../../monte-carlo-estimator.md); correlated simulation output requires a [long-run variance of a stationary process](../../../../../../long-run-variance-of-a-stationary-process.md) estimate instead of the iid [sample variance](../../../../../../sample-variance.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
