<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work in discounted units with a riskless asset of value one, trivial initial information and finitely many risky assets. Let $Y=S_1-S_0\in L^2(P;\mathbb R^d)$ be their discounted gains. A terminal [attainable claim](../../../../../attainable-european-contingent-claim.md) has the form $v+\theta^TY$, whose initial cost is $v$. Their span

$$
\mathcal H=\operatorname{span}\{1,Y_1,\ldots,Y_d\}\subseteq L^2(P)
$$

is a finite-dimensional closed subspace of a [Hilbert space](../../../../../hilbert-space-split.md). For $H\in L^2(P)$, [one-period least-squares hedging](../../../../../one-period-quadratic-hedge.md) is its [orthogonal projection](../../../../../orthogonal-projection.md) onto $\mathcal H$.

Let $m=\mathbb EY$, $\Sigma=\operatorname{Cov}(Y)$ and $b=\operatorname{Cov}(Y,H)$. Remove redundant risky directions so that $\Sigma$ is invertible. Under absence of [arbitrage](../../../../../arbitrage.md), a gain direction with zero [variance](../../../../../variance-split.md) is a constant and must be zero, so this reduction loses no genuine trading opportunity. For freely chosen capital and holdings, minimizing

$$
\mathbb E(H-v-\theta^TY)^2
$$

first gives $v=\mathbb EH-\theta^Tm$. The remaining centered error is

$$
\operatorname{Var}H-2\theta^Tb+\theta^T\Sigma\theta.
$$

Completing the square yields

$$
\boxed{\theta^*=\Sigma^{-1}b,\quad v^*=\mathbb EH-m^T\Sigma^{-1}b,\quad
\min\mathbb E(H-v-\theta^TY)^2=\operatorname{Var}H-b^T\Sigma^{-1}b.}
$$

The residual $L=H-v^*-(\theta^*)^TY$ satisfies $\mathbb EL=0$ and $\mathbb E[LY]=0$, the [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md). Exact [claim replication](../../../../../claim-replication.md) is possible precisely when this residual is zero. If capital is fixed at $v$, its normal equation instead gives the [fixed-capital quadratic hedge in a one-period market](../../../../../fixed-capital-quadratic-hedge-in-a-one-period-market.md)

$$
\theta(v)=\bigl(\mathbb E[YY^T]\bigr)^{-1}\mathbb E[Y(H-v)].
$$

Thus fixed-capital and freely optimized hedging are distinct problems.

A [dominated martingale measure](../../../../../dominated-martingale-measure.md) is a [probability measure](../../../../../probability-measure.md) $Q\ll P$ with integrable gains and $\mathbb E_QY=0$. Its density $Z$ obeys $Z\ge0$, $\mathbb EZ=1$, $\mathbb E[ZY]=0$. An [equivalent martingale measure](../../../../../risk-neutral-measure.md) additionally has $Z>0$ almost surely. Every such measure prices an attainable discounted claim $v+\theta^TY$ at $v$, but different measures may give different [expectations](../../../../../expected-value.md) to an unattainable claim.

The [minimal martingale measure in a one-period market](../../../../../minimal-martingale-measure-in-a-one-period-market.md) is defined by preserving the mean-zero [martingale](../../../../../martingale-split.md) directions orthogonal to the gain innovation $Y-m$. Among square-integrable densities it is

$$
\boxed{Z_*=1-m^T\Sigma^{-1}(Y-m).}
$$

Indeed $\mathbb EZ_*=1$, $\mathbb E[Z_*Y]=m-\Sigma\Sigma^{-1}m=0$, and for $\mathbb EL=0$, $\mathbb E[L(Y-m)]=0$ we have $\mathbb E[Z_*L]=0$. Conversely preservation of all these orthogonal directions puts $Z$ in $\operatorname{span}\{1,Y-m\}$; normalization and zero gain [expectations](../../../../../expected-value.md) then determine $Z_*$. Any other square-integrable signed pricing density differs from $Z_*$ by a vector in $\mathcal H^\perp$, so $Z_*$ also has the smallest $L^2$ norm. Its evaluation of a claim is

$$
\mathbb E[Z_*H]=\mathbb EH-m^T\Sigma^{-1}b=v^*.
$$

This is the capital of the optimal quadratic hedge, not automatically an arbitrage-free price. The formula may define only a [signed martingale measure](../../../../../signed-martingale-measure.md): $Z_*$ is a genuine dominated measure only if it is nonnegative, and equivalent only if strictly positive. For example, gains $(-1,1,2)$ with [probabilities](../../../../../probability.md) $(1/10,4/5,1/10)$ have $m=9/10$, $\Sigma=49/100$ and $Z_*(2)=-50/49$. Yet [probabilities](../../../../../probability.md) $(11/20,7/20,1/10)$ are all positive and have zero gain mean. Thus absence of arbitrage does not force a positive minimal density.

For the [market completeness](../../../../../complete-market.md) assertion, assume absence of arbitrage and hence existence of an [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q_0$. In finite states this is the usual [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md); the one-period version also holds with finitely many assets on a general [probability](../../../../../probability.md) space. [Market completeness](../../../../../complete-market.md) means that every bounded claim is attainable, equivalently $\mathcal H=L^2(P)$ in this square-integrable setting. We now prove [completeness and uniqueness of dominated martingale measures](../../../../../completeness-and-uniqueness-of-dominated-martingale-measures.md).

If the model is complete, replicate every indicator $\mathbf1_A$. Two [dominated martingale measures](../../../../../dominated-martingale-measure.md) both evaluate it at its unique [claim replication](../../../../../claim-replication.md) cost, and therefore assign every event $A$ the same [probability](../../../../../probability.md). They are identical.

Conversely let $k=\dim\mathcal H$ and suppose the model is incomplete. There exist $k+1$ disjoint events $A_j$ of positive [probability](../../../../../probability.md). Otherwise the [probability](../../../../../probability.md) space would have at most $k$ atoms: any non-atomic positive event could be split to increase the number. Its whole payoff space would then have dimension at most $k$, forcing equality with $\mathcal H$ and [market completeness](../../../../../complete-market.md). Choose a basis $h_1,\ldots,h_k$ of $\mathcal H$. Its members are integrable under $Q_0$, because they are combinations of the constant and the gains. The $k+1$ vectors

$$
\bigl(\mathbb E_{Q_0}[h_i\mathbf1_{A_j}]\bigr)_{i=1}^k\in\mathbb R^k
$$

are linearly dependent. Hence a nonzero bounded $g=\sum_j a_j\mathbf1_{A_j}$ satisfies $\mathbb E_{Q_0}[g h]=0$ for every $h\in\mathcal H$, in particular $h=1,Y_i$. For $0<\varepsilon<1/\|g\|_\infty$, define

$$
\frac{dQ_\pm}{dQ_0}=1\pm\varepsilon g.
$$

These strictly positive densities integrate to one, preserve every gain [expectation](../../../../../expected-value.md), and give distinct [equivalent martingale measures](../../../../../risk-neutral-measure.md). They are also dominated by $P$. Thus uniqueness is impossible in an [incomplete market](../../../../../incomplete-market.md), proving the equivalence under the stated no-arbitrage hypothesis.

That hypothesis is essential. On three positive-probability states, the gain $(0,1,2)$ has the unique [dominated martingale measure](../../../../../dominated-martingale-measure.md), concentrated on the first state, but its attainable span has dimension only two. The market is incomplete and admits arbitrage. This explains why uniqueness among merely dominated [probabilities](../../../../../probability.md) must not be used without an equivalent pricing measure or a no-arbitrage assumption.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
