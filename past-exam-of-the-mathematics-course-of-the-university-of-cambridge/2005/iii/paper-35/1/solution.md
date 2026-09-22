<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Normalize by a riskless [bank account](../../../../../bank-account.md) with $B_0=1$, $B_1=R>0$. For $d$ risky assets let $Y=S_1/R-S_0$ be the vector of discounted gains, and let $H$ denote a discounted square-integrable [contingent claim](../../../../../contingent-claim.md). An initial total capital $x$ and [stock](../../../../../stock.md) holding $\vartheta$ have discounted terminal [portfolio wealth](../../../../../portfolio-wealth.md) $x+\vartheta^TY$: the bank holding finances the initial purchase of the [stocks](../../../../../stock.md). Thus the space of [attainable claims](../../../../../attainable-european-contingent-claim.md) is

$$
\mathcal A=\operatorname{span}\{1,Y^1,\ldots,Y^d\}\subset L^2(P).
$$

It is finite-dimensional and hence closed. The market is [complete market](../../../../../complete-market.md) when every square-integrable claim is in this span; with finitely many assets this is also equivalent to replication of every bounded claim.

A [dominated martingale measure](../../../../../dominated-martingale-measure.md) $Q$ is a probability measure with $Q\ll P$ and $\mathbb E_QY=0$, with the gains integrable under $Q$. Its [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md) satisfies $Z\ge0$, $\mathbb EZ=1$ and $\mathbb E[ZY]=0$. An [equivalent martingale measure](../../../../../risk-neutral-measure.md) has $Z>0$ almost surely. A [signed martingale measure](../../../../../signed-martingale-measure.md) obeys the same normalization and pricing equations without requiring nonnegativity. The distinction matters for quadratic hedging. For the completeness assertion use the usual no-[arbitrage](../../../../../arbitrage.md) hypothesis, expressed here by existence of an [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q_0$.

The unrestricted [one-period quadratic hedge](../../../../../one-period-quadratic-hedge.md) minimizes

$$
\mathbb E(H-x-\vartheta^TY)^2.
$$

Put $m=\mathbb EY$, $C=\operatorname{Cov}(Y)$ and $k=\operatorname{Cov}(Y,H)$. Remove redundant gains so that $C$ is invertible. Differentiating in $x$ gives $x=\mathbb EH-\vartheta^Tm$. The remaining squared error is

$$
\operatorname{Var}(H)-2\vartheta^Tk+\vartheta^TC\vartheta
=\operatorname{Var}(H)-k^TC^{-1}k+(\vartheta-C^{-1}k)^TC(\vartheta-C^{-1}k).
$$

Therefore

$$
\boxed{\vartheta_*=C^{-1}k,\qquad x_*=\mathbb EH-m^TC^{-1}k.}
$$

The residual is orthogonal in $L^2(P)$ to $1$ and every gain, making the fitted claim the [orthogonal projection onto a finite-dimensional subspace](../../../../../orthogonal-projection-onto-a-finite-dimensional-subspace.md) onto $\mathcal A$. Its minimum mean-square error is $\operatorname{Var}(H)-k^TC^{-1}k$, and it vanishes exactly when $H$ is attainable. If initial capital $x$ is fixed instead, the normal equation is

$$
(C+mm^T)\vartheta=k+m(\mathbb EH-x).
$$

This separates hedging with prescribed capital from simultaneous optimization of capital and risky holdings.

The [minimal martingale measure in a one-period market](../../../../../minimal-martingale-measure-in-a-one-period-market.md) is characterized by leaving unchanged the [expectation](../../../../../expected-value.md) of every centered square-integrable $L$ orthogonal to the [martingale](../../../../../martingale-split.md) part $Y-m$. For square-integrable pricing densities this forces $Z-1$ into the span of $Y-m$: the orthogonal complement consists exactly of those $L$. The pricing equation then determines

$$
\boxed{Z_*=1-m^TC^{-1}(Y-m).}
$$

Indeed $\mathbb EZ_*=1$ and $\mathbb E[Z_*Y]=m-CC^{-1}m=0$. For every such orthogonal $L$, $\mathbb E[Z_*L]=0$. Conversely a normalized density preserving all these $L$ must have the displayed form, since its coefficients must satisfy $C\beta=-m$. The least-squares initial capital is consequently $x_*=\mathbb E[Z_*H]$.

For any other square-integrable signed pricing density $Z$, put $L=Z-Z_*$. Both densities price $1$ and all gains, so $L$ is orthogonal to their span, including $Z_*$. Hence

$$
\boxed{\mathbb EZ^2=\mathbb EZ_*^2+\mathbb E(Z-Z_*)^2\ge\mathbb EZ_*^2=1+m^TC^{-1}m.}
$$

Equality holds only when $Z=Z_*$. Densities with infinite second moment cannot improve this finite minimum. This proves the requested minimum over [dominated martingale measures](../../../../../dominated-martingale-measure.md) whenever $Z_*\ge0$, and over all square-integrable [signed martingale measures](../../../../../signed-martingale-measure.md) without that extra condition. If $Z_*>0$, it is also an [equivalent martingale measure](../../../../../risk-neutral-measure.md).

**Absence of arbitrage alone does not guarantee that the minimal density is a probability density.** For a concrete example, let a single discounted gain take values $-1,1,10$ with probabilities $1/10,4/5,1/10$. Then $m=17/10$, $C=801/100$ and $Z_*(10)=-610/801$. Nevertheless pricing probabilities $(109/200,89/200,1/100)$ are strictly positive and give mean gain zero, so an [equivalent martingale measure](../../../../../risk-neutral-measure.md) exists. This is [negative minimal density in an arbitrage-free one-period market](../../../../../negative-minimal-density-in-an-arbitrage-free-one-period-market.md). If the term [martingale](../../../../../martingale-split.md) measure is reserved for probabilities, the printed minimum assertion needs the extra nonnegativity hypothesis; otherwise it is the signed minimum-norm assertion just proved. Minimizing over the nonnegative pricing densities instead is a different constrained projection problem.

Finally, prove [completeness and uniqueness of dominated martingale measures](../../../../../completeness-and-uniqueness-of-dominated-martingale-measures.md). If the market is [complete market](../../../../../complete-market.md), every event indicator can be replicated. Under any [dominated martingale measure](../../../../../dominated-martingale-measure.md), its [expectation](../../../../../expected-value.md) equals its initial discounted cost. Consequently any two such measures agree on every event and are equal; existence is supplied by $Q_0$.

Conversely suppose $\mathcal A$ has dimension $k$ and is a proper subspace of the whole payoff space. Choose $k+1$ disjoint events $A_i$ of positive probability. Such events exist whenever $L^2(P)$ has dimension greater than $k$: otherwise the space has at most $k$ atoms and dimension at most $k$. Let $f_1,\ldots,f_k$ be a basis of $\mathcal A$. The $k+1$ vectors

$$
\bigl(\mathbb E_{Q_0}[f_j\mathbf1_{A_i}]\bigr)_{j=1}^k
$$

are linearly dependent. Choose coefficients $a_i$, not all zero, whose linear combination is zero, and set $h=\sum_i a_i\mathbf1_{A_i}$. It is bounded, not almost surely zero under $Q_0$, and satisfies $\mathbb E_{Q_0}[hf]=0$ for every $f\in\mathcal A$, in particular for $1,Y^1,\ldots,Y^d$. For $0<\varepsilon<\|h\|_\infty^{-1}$ define

$$
\frac{dQ_\pm}{dP}=\frac{dQ_0}{dP}(1\pm\varepsilon h).
$$

These densities are strictly positive, normalized, have zero gain means, and are different. Thus incompleteness contradicts uniqueness, proving

$$
\boxed{\text{Under an equivalent pricing measure, completeness}\iff\text{a unique dominated martingale measure}.}
$$

The existence hypothesis cannot be discarded: with three positive-probability states and gain $Y=0,1,2$, the sole dominated [martingale](../../../../../martingale-split.md) probability concentrates on $Y=0$, yet the two-dimensional attainable space does not span all three states. That market permits [arbitrage](../../../../../arbitrage.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
