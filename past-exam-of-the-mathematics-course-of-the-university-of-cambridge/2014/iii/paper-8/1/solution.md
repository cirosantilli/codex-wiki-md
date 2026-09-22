<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A subspace is [topologically complete](../../../../../topological-completeness.md) if its subspace topology is induced by some complete [metric](../../../../../metric.md). The compatible complete [metric](../../../../../metric.md) need not be the restriction of the displayed ambient [metric](../../../../../metric.md). For example, an open interval is topologically complete although its usual [metric](../../../../../metric.md) is incomplete.

Suppose $\rho$ is a compatible complete [metric](../../../../../metric.md) on $Y$. For each $n\ge1$ and $y\in Y$, choose an ambient [open set](../../../../../open-set.md) $V_{n,y}$ containing $y$, contained in $B_d(y,1/n)$, and with $\rho$-diameter of $V_{n,y}\cap Y$ at most $1/n$. Such sets exist because the two topologies on $Y$ agree. Put $U_n=\bigcup_{y\in Y}V_{n,y}$. Clearly $Y\subseteq\bigcap_nU_n$.

If $x\in\bigcap_nU_n$, choose $y_n\in Y$ with $x\in V_{n,y_n}$. Then $d(x,y_n)<1/n$, so $y_n\to x$ in the ambient [metric](../../../../../metric.md). For fixed $m$, the point $x$ belongs to some open $V_{m,z}$, and eventually all $y_n$ belong to this set. Their pairwise $\rho$-distances are then at most $1/m$. Hence $(y_n)$ is $\rho$-Cauchy, and completeness gives a limit $y\in Y$. Compatibility gives $d(y_n,y)\to0$, forcing $x=y$. Thus

$$
\boxed{Y=\bigcap_{n\ge1}U_n.}
$$

This proves the [G-delta criterion for topological completeness](../../../../../g-delta-criterion-for-topological-completeness.md) in the required direction.

**The converse is true in a complete [metric](../../../../../metric.md) ambient space.** If $Y=\bigcap_nU_n$ with each $U_n$ open in complete $X$, define $a_n(y)=1/d(y,X\setminus U_n)$, omitting any term whose complement is empty. A compatible complete [metric](../../../../../metric.md) on $Y$ is

$$
\boxed{D(y,z)=d(y,z)+\sum_{n\ge1}2^{-n}\min\{1,|a_n(y)-a_n(z)|\}.}
$$

Continuity of each $a_n$ and the uniformly small series tail show that $D$ has the original topology. A $D$-[Cauchy sequence](../../../../../cauchy-sequence.md) is $d$-Cauchy, hence converges to some $x\in X$. For each $n$, its real coordinates $a_n$ form a [Cauchy sequence](../../../../../cauchy-sequence.md) and remain bounded. Since distance to a [closed set](../../../../../closed-set.md) is continuous, $d(x,X\setminus U_n)>0$, so $x\in U_n$ for every $n$. The same coordinate convergence and series-tail argument give convergence in $D$. Thus $D$ is complete.

For the normed-space claim, embed $E$ densely in its norm completion $\widehat E$. Topological completeness and the preceding criterion make $E$ a dense [G-delta set](../../../../../g-delta-set.md) in $\widehat E$, hence [comeagre](../../../../../comeagre-set.md). Every translate $x+E$ is also comeagre. The [Baire category theorem](../../../../../baire-category-theorem.md) in the complete space $\widehat E$ implies that $E\cap(x+E)$ is nonempty. If $z=x+e$ lies in that intersection, then $x=z-e\in E$. This holds for every $x\in\widehat E$, so

$$
\boxed{E=\widehat E\text{ and }E\text{ is a Banach space}.}
$$

This is the [comeagre subgroup completeness argument](../../../../../comeagre-subgroup-completeness-argument.md).

Finally let $B=\{\ell\in E^*: \|\ell\|<1\}$ with its [weak-star topology](../../../../../weak-star-topology.md). Put $r_n=1-1/(n+1)$ and $F_n=\{\ell\in B:\|\ell\|\le r_n\}$. The dual norm is the supremum of the continuous evaluation moduli on the unit ball of $E$, so every $F_n$ is relatively closed. Also $B=\bigcup_nF_n$.

Each $F_n$ has empty relative interior. Given $\ell\in F_n$ and a basic weak-star neighborhood restricting finitely many evaluations on $x_1,\ldots,x_k$, the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) gives a nonzero functional $h$ annihilating their finite-dimensional span, because $E$ is infinite-dimensional. All $\ell+th$ retain those evaluations. Their norm varies continuously with $t$ and becomes unbounded; choose $t$ so that $r_n<\|\ell+th\|<1$. This point lies in the neighborhood inside $B$ but outside $F_n$. Thus $B$ is a nonempty countable union of relatively closed nowhere dense sets and is not a [Baire space](../../../../../baire-space.md). Consequently

$$
\boxed{B\text{ with its weak-star topology is not topologically complete}.}
$$

This [weak-star open dual ball category obstruction](../../../../../weak-star-open-dual-ball-category-obstruction.md) works without assuming that $E$ is separable or that the weak-star ball is metrizable.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
