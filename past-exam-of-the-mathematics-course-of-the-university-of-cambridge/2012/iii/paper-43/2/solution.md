<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [futures contract](../../../../../futures-contract.md) fixes a maturity and underlying quantity, but its quoted delivery price is marked to market: gains and losses from quote changes are settled through the margin account, typically daily. A newly settled position has zero contract value; the quoted futures price is not an upfront purchase price for that position. At maturity the quote equals the spot price. In the continuous-settlement idealization, discounted futures gains must be local [martingales](../../../../../martingale-split.md) under the money-market [risk-neutral measure](../../../../../risk-neutral-measure.md). Thus the quote has zero pricing-measure drift. Assuming the relevant [integrability](../../../../../integrability.md) makes it a true [martingale](../../../../../martingale-split.md), **$\boxed{F_{tT}=\mathbb E_Q[S_T\mid\mathcal F_t]}$.**

This is a [futures pricing](../../../../../futures-pricing.md) formula. In contrast, an unsettled [forward contract](../../../../../forward-contract.md) has delivery quote $\mathbb E_Q[D_{tT}S_T\mid\mathcal F_t]/\mathbb E_Q[D_{tT}\mid\mathcal F_t]$, where $D_{tT}=e^{-\int_t^T r_udu}$. Stochastic [interest rates](../../../../../interest-rate.md) can make the two quotes differ. [Contango](../../../../../contango.md) means the futures quote is above spot for the maturity considered, while [backwardation](../../../../../backwardation.md) means it is below spot; futures curves are correspondingly described as rising or falling when comparing maturities.

For the [Multivariate Ornstein-Uhlenbeck process](../../../../../multivariate-ornstein-uhlenbeck-process.md), multiplication by the [matrix exponential](../../../../../matrix-exponential.md) $e^{At}$ gives $d(e^{At}X_t)=e^{At}dB_t$, hence

$$
\boxed{X_t=e^{-At}X_0+\int_0^t e^{-A(t-u)}dB_u.}
$$

For deterministic $X_0=x_0$, the [Gaussian distribution](../../../../../normal-distribution.md) has mean $e^{-At}x_0$ and [covariance](../../../../../covariance.md)

$$
C_t=\int_0^t e^{-Au}e^{-A^{\mathsf T}u}\,du.
$$

Equivalently $\dot C=I-AC-CA^{\mathsf T}$, $C_0=0$. No symmetry or invertibility of $A$ is required. This [covariance](../../../../../covariance.md) can also be evaluated from a single block [matrix exponential](../../../../../matrix-exponential.md): if the upper-right block of $\exp(t\left(\begin{smallmatrix}-A&I\\0&A^{\mathsf T}\end{smallmatrix}\right))$ is $H_t$, then $C_t=H_te^{-A^{\mathsf T}t}$. If $X_0$ is random, these assertions hold conditionally on $X_0$; the unconditional law need not be Gaussian. A stationary Gaussian law exists when the [eigenvalues](../../../../../eigenvalue.md) of $A$ have positive real parts, but stability is unnecessary for the finite-time formulas.

For $\tau=T-t$, the conditional mean of $X_T$ is $e^{-A\tau}X_t$ and its conditional [covariance](../../../../../covariance.md) is $C_\tau$. The Gaussian exponential-moment formula therefore gives **the explicit quote**

$$
\boxed{F_{tT}=\exp\left(b^{\mathsf T}e^{-A\tau}X_t+\tfrac12 b^{\mathsf T}C_\tau b\right).}
$$

It tends to $e^{b\cdot X_t}=S_t$ as $T\downarrow t$, as required.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
