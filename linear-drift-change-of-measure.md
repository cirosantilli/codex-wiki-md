# Linear drift change of measure

↑ **Parent:** [Girsanov theorem](girsanov-theorem.md)

For constant real $a,b$ and $\sigma>0$, the stochastic exponential with integrand $\theta_t=(a-b)X_t/\sigma$ defines an equivalent [change of measure](change-of-measure.md) on every finite horizon. The [Girsanov theorem](girsanov-theorem.md) then changes the drift of this [linear stochastic differential equation](linear-stochastic-differential-equation.md) from $aX$ to $bX$.

A localization argument verifies the necessary unit expectation. Stop at $\tau_m=\inf\{t:|X_t|\geq m\}$. The stopped integrand is bounded, so its exponential density defines a probability $\mathbb Q_m$. Under this probability the stopped process has drift $bX$; the usual second-moment maximal estimate and [Gronwall inequality](gronwall-inequality.md) give $\mathbb E_{\mathbb Q_m}[\sup_{u\leq T}|X_{u\wedge\tau_m}|^2]\leq C_T$ independent of $m$. Thus $\mathbb Q_m(\tau_m\leq T)\leq C_T/m^2$. On $\{\tau_m>T\}$, the stopped and unstopped densities agree, so the expectation of the unstopped density is at least $\lim_m\mathbb Q_m(\tau_m>T)=1$. A nonnegative local [martingale](martingale-split.md) has expectation at most one, proving equality. The density is strictly positive because each finite-horizon continuous path has finite $\int\theta^2dt$. This establishes equivalence without asserting that the stronger [Novikov condition](novikov-s-condition.md) necessarily holds for every horizon.

## ↑ Ancestors (9)

1. [Girsanov theorem](girsanov-theorem.md)
2. [Doléans-Dade exponential](doleans-dade-exponential.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2021/1/b/solution.md)
- [Pricing equation for a linear asset with additive noise](pricing-equation-for-a-linear-asset-with-additive-noise.md)
