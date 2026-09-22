<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Y=h(U)$ have finite [variance](../../../../../../variance-split.md) $v$ and mean $I$. An independent-sample [Monte Carlo estimator](../../../../../../monte-carlo-estimator.md) has [variance](../../../../../../variance-split.md) $v/N$, so its root-mean-square random error is $\sqrt{v/N}$. Three techniques reduce the [variance](../../../../../../variance-split.md) coefficient rather than changing this ordinary $N^{-1/2}$ rate.

For [antithetic variates](../../../../../../antithetic-variates.md), couple $Y=h(U)$ with $Y'=h(1-U)$ and average the pair. With $M$ independent pairs, the [variance](../../../../../../variance-split.md) is $(v+\operatorname{Cov}(Y,Y'))/(2M)$, compared with $v/(2M)$ for $2M$ independent function evaluations. If $h$ is monotone in a scalar uniform, the [covariance](../../../../../../covariance.md) is nonpositive: for independent uniforms $U,V$,

$$
2\operatorname{Cov}(h(U),h(1-U))
=\mathbb E[(h(U)-h(V))(h(1-U)-h(1-V))]\le0.
$$

Opposite fluctuations therefore cancel. The reduction factor at equal evaluation count is $1+\rho$, where $\rho$ is the paired [correlation coefficient](../../../../../../pearson-correlation-coefficient.md); it can approach zero, but positive [covariance](../../../../../../covariance.md) would make the method worse. This is appropriate for monotone or otherwise negatively coupled payoffs, with cheap complementary paths.

For [control variates](../../../../../../control-variates.md), use a jointly simulated $C$ with known mean $m_C$ and average $Y-\beta(C-m_C)$. It remains an [unbiased estimator](../../../../../../unbiased-estimator.md) for fixed $\beta$, and

$$
\operatorname{Var}(Y-\beta C)=v-2\beta\operatorname{Cov}(Y,C)+\beta^2\operatorname{Var}C.
$$

Completing the square gives $\beta_*=\operatorname{Cov}(Y,C)/\operatorname{Var}C$ and minimal [variance](../../../../../../variance-split.md) $v(1-\rho^2)$. For [contingent claim](../../../../../../contingent-claim.md) simulation, an analytically priced related [financial payoff](../../../../../../contingent-claim-payoff.md), such as a simpler option or discounted terminal [stock](../../../../../../stock.md), can be a useful control. It works best when correlation has large absolute value and simulation of the control adds little cost. A coefficient fixed from an independent pilot keeps the elementary unbiasedness argument valid; estimating it from the same sample can introduce finite-sample bias.

For [stratified sampling](../../../../../../stratified-sampling.md), partition the sampling space into strata $A_h$ of probabilities $p_h$, and independently simulate $N_h$ samples conditional on each stratum. The estimator $\sum_hp_h\bar Y_h$ is unbiased and has [variance](../../../../../../variance-split.md)

$$
\sum_h\frac{p_h^2v_h}{N_h},\qquad v_h=\operatorname{Var}(Y\mid A_h).
$$

With proportional allocation $N_h=Np_h$, ignoring integer rounding, this equals $\sum_hp_hv_h/N$. The [law of total variance](../../../../../../law-of-total-variance.md) shows the reduction from ordinary sampling is $\operatorname{Var}(\mathbb E[Y\mid A_h])/N$: fixed representation removes randomness in the stratum counts. At equal per-draw cost, minimizing the displayed [variance](../../../../../../variance-split.md) gives $N_h\propto p_h\sqrt{v_h}$ and minimum $(\sum_hp_h\sqrt{v_h})^2/N$ for positive within-stratum [variances](../../../../../../variance-split.md). This follows by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and is useful when a low-dimensional coordinate strongly predicts the [financial payoff](../../../../../../contingent-claim-payoff.md) and conditional simulation is easy.

**There is no universal ranking.** At comparable cost the [variance](../../../../../../variance-split.md) factors depend respectively on paired [covariance](../../../../../../covariance.md), squared control correlation, and within-stratum variation. A nearly perfect control can outperform a weak antithetic pair; an appropriate stratification can be almost exact for a nearly stratum-constant [financial payoff](../../../../../../contingent-claim-payoff.md). Extra construction and sampling costs must be included in a fair accuracy comparison, and the methods can be combined.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
