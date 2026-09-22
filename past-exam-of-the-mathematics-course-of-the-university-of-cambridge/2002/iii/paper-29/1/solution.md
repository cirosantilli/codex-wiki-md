<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Normalize the riskless [financial asset](../../../../../financial-asset.md) to $B_0=1$, $B_1=b>0$, and write $S_0,S_1$ for the $s$ risky asset prices. Their discounted gain [random vector](../../../../../random-vector.md) is $Y=S_1/b-S_0$. A zero-cost [portfolio](../../../../../investment-portfolio.md) holding $h\in\mathbb R^s$ in the risky assets and $-h\cdot S_0$ in the riskless asset has terminal value $b\,h\cdot Y$. Thus an [arbitrage](../../../../../arbitrage.md) means

$$
h\cdot Y\geq0\quad\text{almost surely},\qquad \mathbb P(h\cdot Y>0)>0.
$$

An [equivalent martingale measure](../../../../../risk-neutral-measure.md) is a [probability measure](../../../../../probability-measure.md) $Q$ with the same [null sets](../../../../../null-set.md) as $P$, under which $Y$ is [integrable](../../../../../integrability.md) and $\mathbb E_QY=0$. The discounted risky prices are then [martingales](../../../../../martingale-split.md) over the single trading period.

If such $Q$ exists, a nonnegative terminal gain has [expectation](../../../../../expected-value.md) zero under $Q$. A nonnegative [random variable](../../../../../random-variable-split.md) with zero [expectation](../../../../../expected-value.md) vanishes [almost surely](../../../../../almost-sure-convergence.md): on $\{X\geq1/n\}$ its [expectation](../../../../../expected-value.md) is at least $\mathbb P(X\geq1/n)/n$, and the union of these events is $\{X>0\}$. Equivalence transfers this conclusion to $P$, excluding [arbitrage](../../../../../arbitrage.md).

For the converse we prove the needed [positive-density separation proof of the one-period asset-pricing theorem](../../../../../positive-density-separation-proof-of-the-one-period-asset-pricing-theorem.md). First make the gain [integrable](../../../../../integrability.md) without changing its [null sets](../../../../../null-set.md). Define an [equivalent probability measure](../../../../../equivalent-probability-measure.md) $P_0$ by

$$
\frac{dP_0}{dP}=\frac{k}{1+\|Y\|},\qquad
k^{-1}=\mathbb E_P\frac1{1+\|Y\|}.
$$

Let $N=\{h:h\cdot Y=0\text{ almost surely}\}$ and let $L=N^\perp$ be its [orthogonal complement](../../../../../orthogonal-complement.md). Taking a finite [basis](../../../../../basis.md) of $N$ shows $Y\in L$ [almost surely](../../../../../almost-sure-convergence.md). If $L=\{0\}$, the gain is zero and $P_0$ already gives the required measure. Otherwise consider the [positive-weight expectation cone](../../../../../positive-weight-expectation-cone.md)

$$
C=\{\mathbb E_{P_0}[ZY]: Z\text{ bounded and }Z>0\text{ almost surely}\}\subset L.
$$

Positive combinations of weights show that $C$ is a [convex cone](../../../../../convex-cone.md). It is open relative to $L$. Indeed, for any admissible weight $Z$, perturb it to

$$
Z_\varepsilon=Z\left(1+\frac{\varepsilon\cdot Y}{1+\|Y\|}\right),\qquad \varepsilon\in L,\quad \|\varepsilon\|<1.
$$

These weights remain bounded and strictly positive, while

$$
\mathbb E_{P_0}[Z_\varepsilon Y]=\mathbb E_{P_0}[ZY]+A_Z\varepsilon,
\qquad A_Z=\mathbb E_{P_0}\frac{ZYY^T}{1+\|Y\|}.
$$

For every nonzero $v\in L$, $v\cdot Y$ is nonzero on an event of positive [probability](../../../../../probability.md); otherwise $v\in N\cap L$. Consequently

$$
v^TA_Zv=\mathbb E_{P_0}\frac{Z(v\cdot Y)^2}{1+\|Y\|}>0.
$$

The [matrix](../../../../../matrix.md) is finite because $\|Y\|^2/(1+\|Y\|)\leq\|Y\|$. The [kernel](../../../../../kernel-of-a-linear-map.md) of $A_Z$ on $L$ is zero, so it defines an [invertible matrix](../../../../../invertible-matrix.md) on the [finite-dimensional vector space](../../../../../finite-dimensional-vector-space.md) $L$. For any sufficiently small $\delta>0$, every $y$ with $\|y\|<\delta/\|A_Z^{-1}\|$ is the image of a vector in the radius-$\delta$ ball, since $\|A_Z^{-1}y\|<\delta$. Hence the perturbations give a [neighborhood](../../../../../neighbourhood-mathematics.md) of zero, proving relative openness of $C$.

If $0\notin C$, the [hyperplane separation theorem](../../../../../hyperplane-separation-theorem.md) gives a nonzero $h\in L$ with $h\cdot c\geq0$ for every $c\in C$. The separating constant can be taken to be zero because $C$ is a cone. Put $A=\{h\cdot Y<0\}$ and use the strictly positive weights $Z=\mathbf1_A+\varepsilon$. Taking the [limit](../../../../../limit-of-a-function.md) as $\varepsilon\downarrow0$ yields $\mathbb E_{P_0}[(h\cdot Y)\mathbf1_A]\geq0$, forcing $P_0(A)=0$. But $h\notin N$, so $P_0(h\cdot Y>0)>0$. This is an [arbitrage](../../../../../arbitrage.md), a contradiction. Hence $0\in C$: some bounded strictly positive $Z$ satisfies $\mathbb E_{P_0}[ZY]=0$. Normalize it by $dQ/dP_0=Z/\mathbb E_{P_0}Z$. This gives an [equivalent martingale measure](../../../../../risk-neutral-measure.md) with [integrable](../../../../../integrability.md) gains, establishing the [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md) here without any further existence theorem.

Now retain only the $m$ positive-probability states of the finite [probability space](../../../../../probability-space.md). Let $V\subseteq\mathbb R^m$ be the [linear span](../../../../../linear-span.md) of the discounted terminal asset payoffs; it contains the constant vector $\mathbf1$. A [complete market](../../../../../complete-market.md) means $V=\mathbb R^m$. An [equivalent martingale measure](../../../../../risk-neutral-measure.md) is a vector $q$ of strictly positive state probabilities whose pairing with each asset payoff gives its initial price. By linearity it prices every attainable payoff. If $V=\mathbb R^m$, the [indicator functions](../../../../../indicator-function.md) of individual states are attainable, so these prices determine every $q_j$ uniquely.

If $V$ is proper, choose $0\ne v\in V^\perp$. Since $\mathbf1\in V$, $\sum_jv_j=0$. For sufficiently small $\varepsilon>0$, both $q+\varepsilon v$ and $q-\varepsilon v$ have strictly positive entries, sum to one, and give the same pairings with every asset payoff. They are distinct [equivalent martingale measures](../../../../../risk-neutral-measure.md). Therefore [market completeness](../../../../../complete-market.md) is equivalent to uniqueness of the [equivalent martingale measure](../../../../../risk-neutral-measure.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
