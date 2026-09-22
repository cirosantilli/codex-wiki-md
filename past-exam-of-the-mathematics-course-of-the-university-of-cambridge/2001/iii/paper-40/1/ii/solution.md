<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The independent dimensionless variable is $S=s/s_\infty$. Since $gZ_i=s_\infty GZ_i$ and $dS/ds=1/s_\infty$, the chain rule gives $d(gZ_i)/ds=d(GZ_i)/dS$. The derivative in the normalized equation must consequently be with respect to $S$. Substituting the gas history in the [retained-ejecta chemical evolution](../../../../../../retained-ejecta-chemical-evolution.md) equation yields

$$
\frac{d(GZ_i)}{dS}+\frac{1-\beta f}{(1-\beta)S(1-S)}GZ_i=y_if.
$$

This step allows a varying retention fraction $f(S)$; no derivative of $f$ is needed because $f$ enters the instantaneous metal source and loss terms.

Set $H=GZ_i$ and now take $f=S$. The coefficient in this first-order [ordinary differential equation](../../../../../../ordinary-differential-equation.md) decomposes as

$$
\frac{1-\beta S}{(1-\beta)S(1-S)}=\frac1{(1-\beta)S}+\frac1{1-S}.
$$

Hence an [integrating factor](../../../../../../integrating-factor.md) is $\mu(S)=S^{1/(1-\beta)}/(1-S)$. With $q=1+1/(1-\beta)=(2-\beta)/(1-\beta)$, multiplication by this [integrating factor](../../../../../../integrating-factor.md) gives

$$
\mu H=S^qZ_i,
\qquad
\frac d{dS}(S^qZ_i)=\frac{y_iS^q}{1-S}.
$$

The general solution has an additional term $C/S^q$. Finite initial [gas-phase metallicity](../../../../../../gas-phase-metallicity.md) rules it out. Consequently, for $0<S<1$,

$$
\boxed{Z_i(S)=\frac{y_i}{S^q}\int_0^S\frac{u^q}{1-u}\,du.}
$$

The upper limit is the dimensionless $S$, not the unnormalized stellar mass. On each compact subinterval of $0\leq S<1$, the [geometric series](../../../../../../geometric-series.md) $1/(1-u)=\sum_{k\geq0}u^k$ converges uniformly, permitting integration term by term. Thus

$$
Z_i=\frac{y_i}{S^q}\sum_{k=0}^{\infty}\frac{S^{q+k+1}}{q+k+1}
=\boxed{y_i\sum_{n=1}^{\infty}\frac{S^n}{q+n}.}
$$

In particular $Z_i\sim y_iS/(q+1)$ at small $S$. For positive [stellar yield](../../../../../../stellar-yield.md), the series is strictly increasing, so the inverse needed for the [metallicity distribution function](../../../../../../metallicity-distribution-function.md) exists. Differentiating either representation gives $Z_i'=y_i/(1-S)-qZ_i/S>0$. It diverges logarithmically as gas exhaustion approaches; the trace-metal approximation eventually becomes inadequate.

The [quadratic gas-history enrichment model](../../../../../../quadratic-gas-history-enrichment-model.md) is not a closed gas reservoir: its gas mass initially increases. This can be made consistent with the metal equation by pristine [galactic gas inflow](../../../../../../galactic-gas-inflow.md). Indeed gas accounting gives $dg/ds=-(1-\beta f)/(1-\beta)+dM_{\rm in}/ds$. Since $dg/ds=1-2S$ and $f=S$, the required inflow is $dM_{\rm in}/ds=q(1-S)\geq0$. It adds no metals and therefore leaves the preceding derivation intact.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
