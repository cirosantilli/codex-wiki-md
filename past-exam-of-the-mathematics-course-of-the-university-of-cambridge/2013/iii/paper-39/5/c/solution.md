<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [spot interest rate](../../../../../../spot-interest-rate.md) $r_T$ is known at $T-1$. The [state-price density](../../../../../../state-price-density.md) price of its floating payment is, by the [law of total expectation](../../../../../../law-of-total-expectation.md),

$$
\begin{aligned}
\frac1{Z_0}\mathbb E[Z_T r_T]
&=\frac1{Z_0}\mathbb E\left[Z_{T-1}P_{T-1}(T)\left(\frac1{P_{T-1}(T)}-1\right)\right]\\
&=P_0(T-1)-P_0(T).
\end{aligned}
$$

Here $P_0(0)=1$ if $T=1$. All these terms are integrable: $Z_Tr_T$ is bounded in absolute value by $Z_T/P_{T-1}(T)+Z_T$, whose expectation is finite from the one-step pricing relation. Subtracting the fixed payment $f$ gives

$$
\xi_0=P_0(T-1)-(1+f)P_0(T),
\qquad
\boxed{f=\frac{P_0(T-1)}{P_0(T)}-1\ \Longrightarrow\ \xi_0=0.}
$$

This also follows directly from a [floating-rate payment bond replication](../../../../../../floating-rate-payment-bond-replication.md). At time zero buy one unit of the bond maturing at $T-1$ and short $1+f$ units of the bond maturing at $T$. Their initial cost is the displayed $\xi_0$. Hold them until $T-1$. The first bond then pays one; spend that one to buy $1/P_{T-1}(T)$ units of the maturity-$T$ bond, leaving the earlier short position in place. This rebalance is [self-financing](../../../../../../self-financing-portfolio.md). At maturity the net payment is

$$
\frac1{P_{T-1}(T)}-(1+f)=r_T-f.
$$

For $T=1$, the first unit is time-zero cash, and the same immediate rebalance gives the deterministic payoff. Thus the replication establishes the zero no-arbitrage price without requiring completeness of other claims.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
