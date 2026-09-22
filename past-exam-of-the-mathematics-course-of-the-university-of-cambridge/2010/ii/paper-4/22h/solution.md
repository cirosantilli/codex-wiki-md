<h1 id="22h/solution">Solution</h1>

↑ **Parent:** [22H](../22h.md)

A bounded linear operator is [compact](../../../../../compact-space.md) if it maps the unit ball to a set with compact closure; equivalently, every bounded sequence has a subsequence whose images converge.

If $S,T$ are [compact operators](../../../../../compact-operator-split.md), select a subsequence on which $Sx_n$ converges and then a further subsequence on which $Tx_n$ converges. This proves [compactness](../../../../../compact-space.md) of any [linear combination](../../../../../linear-combination.md). For norm closure, suppose compact $T_j$ converge to $T$ in [operator norm](../../../../../operator-norm.md). Given $\varepsilon>0$, choose $j$ with $\|T-T_j\|<\varepsilon/3$. A finite $\varepsilon/3$-net for $T_j$ of the unit ball is then a finite $2\varepsilon/3$-net for its image under $T$. This image is totally bounded, and its closure is compact because $X$ is complete. Thus $B_0(X)$ is a closed linear subspace.

For bounded $S$ and compact $T$, the image of a bounded sequence under $S$ is bounded, so $TS$ is compact; and a convergent subsequence of $Tx_n$ remains convergent after applying the continuous map $S$, so $ST$ is compact. Therefore **the [compact operators](../../../../../compact-operator-split.md) form a closed two-sided ideal in $B(X)$**.

For the weighted backward shift, truncate its output after coordinate $N$, obtaining a finite-rank operator $T_N$. The exact norm estimate is

$$
\|T-T_N\|=\sup_{k>N}\frac1{k+1}=\frac1{N+2}\to0.
$$

Hence $T$ is compact. Its iterates are

$$
(T^mx)_k=\frac{x_{k+m}}{(k+1)(k+2)\cdots(k+m)},\qquad
\|T^m\|=\frac1{(m+1)!}.
$$

Thus for every nonzero complex $\lambda$ the [Neumann series](../../../../../neumann-series.md)

$$
(\lambda I-T)^{-1}
=\sum_{m\ge0}\lambda^{-m-1}T^m
$$

converges absolutely in [operator norm](../../../../../operator-norm.md). Zero is an [eigenvalue](../../../../../eigenvalue.md), since $Te_1=0$, whereas every nonzero value is in the resolvent set. Consequently

$$
\boxed{T\text{ is compact},\qquad \sigma(T)=\{0\}.}
$$

## ↑ Ancestors (10)

1. [22H](../22h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
