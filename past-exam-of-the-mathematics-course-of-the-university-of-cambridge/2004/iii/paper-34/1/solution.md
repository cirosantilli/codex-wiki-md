<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the riskless [financial asset](../../../../../financial-asset.md) as [numéraire](../../../../../numeraire.md), normalized to have initial value one and terminal value $R>0$. Write $S_0\in\mathbb R^s$ for the initial risky prices and $S_1$ for the finite, measurable terminal price [random vector](../../../../../random-vector.md). Define the discounted gain vector $X=S_1/R-S_0$. A risky holding $h$ financed by the cash holding $-h\cdot S_0$ has zero initial cost and discounted terminal gain $h\cdot X$. An [arbitrage](../../../../../arbitrage.md) is such a [portfolio](../../../../../investment-portfolio.md) with $h\cdot X\geq0$ almost surely and $\mathbb P(h\cdot X>0)>0$. Allowing nonpositive initial cost is equivalent: invest any initial surplus in the riskless [financial asset](../../../../../financial-asset.md) to obtain a zero-cost [arbitrage](../../../../../arbitrage.md).

An [equivalent martingale measure](../../../../../risk-neutral-measure.md) is a [probability measure](../../../../../probability-measure.md) $Q$ with exactly the same null events as the physical [probability measure](../../../../../probability-measure.md) $P$, under which discounted asset prices are integrable and satisfy $\mathbb E_Q[S_1/R]=S_0$. Equivalently, $\mathbb E_QX=0$. Such a measure rules out [arbitrage](../../../../../arbitrage.md): every zero-cost [portfolio](../../../../../investment-portfolio.md) has mean discounted gain zero, whereas a nonnegative gain positive with positive $P$-probability is also positive with positive $Q$-probability and has strictly positive $Q$-expectation.

For the converse, the [probability space](../../../../../probability-space.md) need not be finite, and the payoffs need not be integrable under $P$. Here is a direct [Gaussian-damped martingale density construction](../../../../../gaussian-damped-martingale-density-construction.md). Set

$$
N=\{h\in\mathbb R^s:h\cdot X=0\text{ almost surely}\},\qquad L=N^\perp,\qquad F(h)=\mathbb E_P e^{-|X|^2-h\cdot X}\quad(h\in L).
$$

The set $N$ is a [linear subspace](../../../../../vector-subspace.md). Choosing a finite [basis](../../../../../basis.md) of $N$ shows that $X\in L$ almost surely: intersect the probability-one events on which each basis vector is orthogonal to $X$. If $h\in L\setminus\{0\}$, then $h\cdot X$ is not almost surely zero. Absence of [arbitrage](../../../../../arbitrage.md) implies both $P(h\cdot X<0)>0$ and $P(h\cdot X>0)>0$, by applying the definition to $h$ and $-h$.

All the analytical steps in minimizing $F$ can be checked directly. On $|h|\leq H$ the integrand is bounded by $e^{H^2/4}$, since $-|X|^2+H|X|\leq H^2/4$. Its first two directional [derivatives](../../../../../derivative.md) are bounded uniformly in $X$ by constants depending only on $H$ and the direction, because the functions $r^j e^{-r^2+(H+1)r}$ are bounded for $j=0,1,2$. The mean-value bound therefore proves continuity of $F$, and the [Taylor theorem](../../../../../taylor-theorem.md) remainder bound, integrated over $P$, proves

$$
D_vF(h)=-\mathbb E_P[(v\cdot X)e^{-|X|^2-h\cdot X}],\qquad v\in L.
$$

Thus differentiation under the integral does not require an unproved physical moment assumption.

To prove [coercivity](../../../../../coercive-function.md), suppose $|h_k|\to\infty$ in $L$. A subsequence of $h_k/|h_k|$ converges to a unit vector $v\in L$. This elementary finite-dimensional [compactness](../../../../../compact-space.md) follows by successively taking convergent subsequences of the bounded coordinates. Since $P(v\cdot X<0)>0$, some event $A=\{v\cdot X\leq-\varepsilon,\ |X|\leq K\}$ has positive [probability](../../../../../probability.md): the negative-gain event is the countable union of such events with $\varepsilon=1/j$ and integer $K$. Eventually $(h_k/|h_k|)\cdot X\leq-\varepsilon/2$ on $A$, and hence

$$
F(h_k)\geq P(A)e^{-K^2}e^{|h_k|\varepsilon/2}\longrightarrow\infty.
$$

If [coercivity](../../../../../coercive-function.md) failed, an unbounded sequence with bounded $F$ would have just such a contradictory subsequence. Consequently a minimizing sequence for $F$ is bounded and has a convergent subsequence; continuity makes its limit $h_*$ a minimizer. If $L=\{0\}$, simply take $h_*=0$. In every case the directional [derivatives](../../../../../derivative.md) vanish at $h_*$. The vector $\mathbb E_P[Xe^{-|X|^2-h_*\cdot X}]$ lies in $L$ and is orthogonal to $L$, so it is zero. Therefore

$$
\boxed{\frac{dQ}{dP}=\frac{e^{-|X|^2-h_*\cdot X}}{\mathbb E_Pe^{-|X|^2-h_*\cdot X}}}
$$

is a positive mean-one density defining an [equivalent martingale measure](../../../../../risk-neutral-measure.md). Integrability of $X$ under $Q$ follows from the same Gaussian bound with $j=1$. This establishes **absence of arbitrage if and only if an equivalent martingale measure exists**, without quoting a financial duality theorem or assuming a finite state space.

Now suppose the [probability space](../../../../../probability-space.md) is finite. Discard null states and enumerate its positive-probability atoms by $1,\ldots,m$. Every measurable terminal payoff is a vector in $\mathbb R^m$. Let $A$ be the $m\times(s+1)$ [matrix](../../../../../matrix.md) whose columns are the discounted terminal payoffs of the traded [financial assets](../../../../../financial-asset.md), with first column $\mathbf1$, and let $p=(1,S_0)$ be their initial price vector. A [portfolio](../../../../../investment-portfolio.md) with holding vector $z$ replicates the discounted payoff $Az$, and an [equivalent martingale measure](../../../../../risk-neutral-measure.md) is exactly a vector $q$ satisfying

$$
q_j>0,\qquad A^Tq=p.
$$

The first pricing equation includes $\sum_jq_j=1$. A [complete market](../../../../../complete-market.md) means $\operatorname{im}A=\mathbb R^m$. If $q,q'$ both price the [financial assets](../../../../../financial-asset.md), then $(q-q')\cdot Az=0$ for every $z$. Completeness allows $Az$ to be each coordinate vector, so $q=q'$.

Conversely, if the [financial market](../../../../../financial-market.md) is incomplete, there is a nonzero vector $v$ with $A^Tv=0$. To see this without invoking a duality theorem, perform row elimination on the homogeneous system: its number of pivots is $\operatorname{rank}A<m$, leaving a free variable and hence a nonzero solution. The constant payoff column gives $\sum_jv_j=0$. Existence of an [equivalent martingale measure](../../../../../risk-neutral-measure.md) was already proved, so choose one strictly positive vector $q$. For

$$
0<\varepsilon<\min_{v_j\ne0}\frac{q_j}{|v_j|},
$$

both $q+\varepsilon v$ and $q-\varepsilon v$ are distinct strictly positive probability vectors satisfying $A^T(q\pm\varepsilon v)=p$. Thus uniqueness fails. **On a finite arbitrage-free market, completeness is equivalent to uniqueness of the equivalent martingale measure.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
