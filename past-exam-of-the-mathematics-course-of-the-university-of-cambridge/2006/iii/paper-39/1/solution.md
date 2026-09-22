<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a strictly positive [bank account](../../../../../bank-account.md) as [numéraire](../../../../../numeraire.md), and write all prices and payoffs in discounted units. There are $d$ risky assets with deterministic initial price vector $S_0$, terminal price vector $S_1\in L^2(P)$, and gains $Y=S_1-S_0$. A [self-financing portfolio](../../../../../self-financing-portfolio.md) with initial capital $x$ and constant risky holdings $\theta$ has discounted terminal wealth $x+\theta^TY$. The initial amount in the [bank account](../../../../../bank-account.md) is $x-\theta^TS_0$, so $x$ denotes total initial capital, not just the cash holding. Assume the usual absence of [arbitrage](../../../../../arbitrage.md), and hence existence of an [equivalent martingale measure](../../../../../risk-neutral-measure.md); wherever a general [probability space](../../../../../probability-space.md) is used below, explicitly assume that such a measure exists and makes the asset payoffs integrable.

The [attainable claims](../../../../../attainable-european-contingent-claim.md) are precisely the [linear subspace](../../../../../vector-subspace.md)

$$
\mathcal A=\operatorname{span}\{1,Y_1,\ldots,Y_d\}\subset L^2(P).
$$

The [finite-dimensional subspace is closed](../../../../../finite-dimensional-subspace-is-closed.md), so every [square-integrable](../../../../../square-integrable-function.md) [contingent claim](../../../../../contingent-claim.md) $H$ has a unique [orthogonal projection](../../../../../orthogonal-projection.md) onto $\mathcal A$. This is its optimal [one-period least-squares hedging](../../../../../one-period-quadratic-hedge.md) payoff. Holdings are unique after redundant assets have been removed. Put

$$
m=\mathbb E_PY,\qquad C=\operatorname{Cov}_P(Y),\qquad c_H=\operatorname{Cov}_P(Y,H),
$$

and suppose the remaining [covariance matrix](../../../../../covariance-matrix.md) $C$ is invertible. Expanding the squared error gives

$$
\mathbb E_P(H-x-\theta^TY)^2
=(\mathbb E_PH-x-\theta^Tm)^2+\operatorname{Var}_P(H)-2\theta^Tc_H+\theta^TC\theta.
$$

First minimize over $x$, then complete the square in $\theta$. Thus

$$
\boxed{\theta_*=C^{-1}c_H,\qquad x_*=\mathbb E_PH-m^TC^{-1}c_H.}
$$

The residual $L=H-x_*-\theta_*^TY$ satisfies

$$
\mathbb E_PL=0,\qquad\mathbb E_P[YL]=0,
\qquad\min_{x,\theta}\mathbb E_P(H-x-\theta^TY)^2
=\operatorname{Var}_P(H)-c_H^TC^{-1}c_H.
$$

Indeed, every other squared error equals this minimum plus

$$
(x-x_*+(\theta-\theta_*)^Tm)^2+(\theta-\theta_*)^TC(\theta-\theta_*).
$$

This proves optimality, and also shows that zero error is equivalent to [attainability of a European contingent claim](../../../../../attainable-european-contingent-claim.md). If initial capital $x$ is prescribed instead, the [normal equations for linear least squares](../../../../../normal-equations-for-linear-least-squares.md) give $\mathbb E[YY^T]\theta=\mathbb E[Y(H-x)]$; one must not use the free-capital formula without this adjustment.

A [dominated martingale measure](../../../../../dominated-martingale-measure.md) is a [probability measure](../../../../../probability-measure.md) $Q\ll P$ such that $\mathbb E_QY=0$. Its [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md) $Z$ satisfies $Z\geq0$, $\mathbb E_PZ=1$, and $\mathbb E_P[ZY]=0$. An [equivalent martingale measure](../../../../../risk-neutral-measure.md) additionally requires $Z>0$ almost surely. Every integrable [attainable claim](../../../../../attainable-european-contingent-claim.md) $H=x+\theta^TY$ then has price $x=\mathbb E_QH$, independent of which such measure is chosen. For an unattainable [contingent claim](../../../../../contingent-claim.md), different [dominated martingale measures](../../../../../dominated-martingale-measure.md) can give different prices; least-squares approximation chooses a projection criterion rather than exact replication.

Write $Y=m+M$, where $M=Y-m$ is the centered [martingale](../../../../../martingale-split.md) part of the one-period gains. The [minimal martingale measure in a one-period market](../../../../../minimal-martingale-measure-in-a-one-period-market.md) changes the means of the traded gains to zero while preserving all [square-integrable](../../../../../square-integrable-function.md) mean-zero directions $L$ [orthogonal](../../../../../orthogonal-vectors.md) to $M$. Its candidate density is

$$
\boxed{Z_*=1-m^TC^{-1}(Y-m).}
$$

Direct computation gives $\mathbb E_PZ_*=1$ and $\mathbb E_P[Z_*Y]=m-CC^{-1}m=0$. If $\mathbb E_PL=0$ and $\mathbb E_P[ML]=0$, then $\mathbb E_P[Z_*L]=0$, as required. Conversely, an $L^2$ density with this preservation property is [orthogonal](../../../../../orthogonal-vectors.md) to the [orthogonal complement](../../../../../orthogonal-complement.md) of $\operatorname{span}\{1,M_1,\ldots,M_d\}$, so it lies in that span. Its normalization and [martingale](../../../../../martingale-split.md) constraints force exactly $Z_*$. Moreover,

$$
x_*=\mathbb E_P[Z_*H].
$$

Every other [square-integrable](../../../../../square-integrable-function.md) signed pricing density has the form $Z_*+D$, with $D$ [orthogonal](../../../../../orthogonal-vectors.md) to $1$ and $Y$, hence to $Z_*$. Therefore

$$
\mathbb E_P[(Z_*+D)^2]=\mathbb E_PZ_*^2+\mathbb E_PD^2,
$$

so the minimal density is also the [minimum-norm one-period pricing weight](../../../../../minimum-norm-one-period-pricing-weight.md). This coincidence concerns one period; it is not an unrestricted assertion about dynamic hedging models.

Positivity needs checking. If $Z_*>0$ it defines an [equivalent martingale measure](../../../../../risk-neutral-measure.md); if merely $Z_*\geq0$, it defines a [dominated martingale measure](../../../../../dominated-martingale-measure.md). Otherwise it defines only a [signed martingale measure](../../../../../signed-martingale-measure.md). For example, take $S_0=2$ and $Y=-1,1,3$ with physical probabilities $1/100,89/100,10/100$. Then $m=59/50$, $C=1019/2500$, and $Z_*=-4350/1019$ in the third state. There is nonetheless an [equivalent martingale measure](../../../../../risk-neutral-measure.md) assigning probabilities $3/5,3/10,1/10$, whose mean gain is zero. Thus absence of [arbitrage](../../../../../arbitrage.md) does not guarantee positivity of the least-squares density, and a least-squares initial cost need not be an arbitrage-free price for an unattainable payoff.

Finally prove [completeness and uniqueness of dominated martingale measures](../../../../../completeness-and-uniqueness-of-dominated-martingale-measures.md). Suppose first that every bounded [contingent claim](../../../../../contingent-claim.md) is attainable. For any event $A$, replicate $\mathbf1_A=x_A+\theta_A^TY$. Under any [dominated martingale measure](../../../../../dominated-martingale-measure.md), $Q(A)=x_A$. Thus all such measures agree on every event. Existence follows from our no-arbitrage assumption, giving uniqueness.

Conversely, fix an [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q_0$, and let $k=\dim\mathcal A$. If the [probability space](../../../../../probability-space.md) admits $k+1$ disjoint events $A_1,\ldots,A_{k+1}$ of positive probability, choose a basis $a_1,\ldots,a_k$ of $\mathcal A$, including $1$. The $k\times(k+1)$ matrix with entries $\mathbb E_{Q_0}[a_i\mathbf1_{A_j}]$ has a nonzero null vector $(c_j)$. Consequently the bounded, nonzero [random variable](../../../../../random-variable-split.md)

$$
h=\sum_{j=1}^{k+1}c_j\mathbf1_{A_j}
$$

satisfies $\mathbb E_{Q_0}h=0$ and $\mathbb E_{Q_0}[hY]=0$. For $0<|\varepsilon|<1/\|h\|_\infty$, define

$$
\frac{dQ_\varepsilon}{dQ_0}=1+\varepsilon h.
$$

These are distinct [equivalent martingale measures](../../../../../risk-neutral-measure.md), because their densities are positive and their gain moments remain zero. Thus uniqueness rules out such a partition. A [probability space](../../../../../probability-space.md) with no $k+1$ disjoint positive-probability events consists, modulo null sets, of at most $k$ atoms: repeatedly split any non-atomic positive event to obtain a larger finite partition. On $N$ atoms the payoff space has dimension $N$, while $\mathcal A$ has dimension $k\leq N$. Hence $N=k$ and $\mathcal A$ is the whole payoff space. Every [contingent claim](../../../../../contingent-claim.md) is attainable. This proves

$$
\boxed{\text{complete, arbitrage-free one-period market}\quad\Longleftrightarrow\quad\text{unique dominated martingale measure}.}
$$

Here completeness means all bounded claims, or all [square-integrable](../../../../../square-integrable-function.md) claims in the $L^2$ formulation. The existence/no-arbitrage hypothesis matters: on a one-state space, cash and a [stock](../../../../../stock.md) with a sure positive discounted gain span every payoff, but no [dominated martingale measure](../../../../../dominated-martingale-measure.md) can make that gain have zero mean.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
