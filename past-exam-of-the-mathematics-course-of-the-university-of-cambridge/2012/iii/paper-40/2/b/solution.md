<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\overline F(M)=1-F_X(M)$. The [compound Poisson distribution](../../../../../../compound-poisson-distribution.md) [variance](../../../../../../variance-split.md) identity and the per-claim [excess of loss reinsurance](../../../../../../excess-of-loss-reinsurance.md) payouts give

$$
g(M)=\lambda\left[\int_0^M x^2f_X(x)\,dx+M^2\overline F(M)
+\int_M^\infty(x-M)^2f_X(x)\,dx\right].
$$

Apply [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md). The endpoint terms $M^2f_X(M)$ in the first two terms cancel, while the last integrand is zero at its lower endpoint. Equivalently, differentiate the two payout squares inside their [expected values](../../../../../../expected-value.md); the finite [second moment](../../../../../../second-moment.md) supplies a dominating integrable function. This gives the [total variance stationary condition for excess of loss](../../../../../../total-variance-stationary-condition-for-excess-of-loss.md)

$$
g'(M)=2\lambda\left[M\overline F(M)-\int_M^\infty(x-M)f_X(x)\,dx\right].
$$

Hence the specified equality makes **$g'(M)=0$**. When $\overline F(M)>0$, its interpretation is $M=m_X(M)$, where the [mean residual life](../../../../../../mean-residual-life.md) is $m_X(M)=\mathbb E[X-M\mid X>M]$.

For the [exponential distribution](../../../../../../exponential-distribution.md) of mean $\mu$, $\overline F(M)=e^{-M/\mu}$ and

$$
\mathbb E[(X-M)_+]=\mu e^{-M/\mu}.
$$

Thus $g'(M)=2\lambda e^{-M/\mu}(M-\mu)$ is negative below $\mu$ and positive above it. The [variance-minimizing exponential retention](../../../../../../variance-minimizing-exponential-retention.md) is the unique global minimizer

$$
\boxed{M^*=\mu.}
$$

For an explicit value, put $m=M/\mu$. The [capped claim moments](../../../../../../capped-claim-moments.md) and the excess-claim [second moment](../../../../../../second-moment.md) give

$$
g(M)=2\lambda\mu^2(1-me^{-m}),\qquad
\boxed{g(\mu)=2\lambda\mu^2(1-e^{-1}).}
$$

The sign argument establishes global minimality, rather than just stationarity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
