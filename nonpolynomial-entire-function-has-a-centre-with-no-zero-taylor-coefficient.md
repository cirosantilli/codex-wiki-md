# Nonpolynomial entire function has a centre with no zero Taylor coefficient

↑ **Parent:** [Baire category theorem](baire-category-theorem.md)

If an [entire function](entire-function.md) $f$ is not a [polynomial](polynomial-split.md), then there is a point $z_0\in\mathbb C$ for which $f^{(n)}(z_0)\ne0$ for every nonnegative integer $n$. Consequently every coefficient in the [Taylor series](taylor-series.md) of $f$ about $z_0$ is nonzero.

For each $n$, the function $f^{(n)}$ is not identically zero, since otherwise $f$ would be a polynomial. Its zero set is closed and has empty interior by the [identity theorem](identity-theorem.md), hence is a [nowhere dense set](nowhere-dense-set.md). The [Baire category theorem](baire-category-theorem.md) says that the [complete metric space](complete-metric-space.md) $\mathbb C$ cannot be the union of these countably many zero sets.

Set $S_n=\{x:f^{(n)}(x)=0\}$ and $E_n=\operatorname{int}S_n$. The sets $S_n$ are closed, $E_n\subset E_{n+1}$, and Baire's theorem on each interval shows that $\Omega=\bigcup_nE_n$ is dense. On every connected component of $\Omega$, compactness and the increasing cover by the $E_n$ show that one derivative vanishes locally with a uniform finite order, so $f$ agrees there with one polynomial.

If $F=\mathbb R\setminus\Omega$ were nonempty, it would be closed and have no isolated points: polynomial pieces on both sides of an isolated point would have matching derivatives of every order and hence join into one polynomial piece. Applying Baire's theorem to the cover $F=\bigcup_n(F\cap S_n)$ gives an interval $U$ and an index $k$ for which $F\cap U$ is nonempty and contained in $S_k$. Because $F$ has no isolated points, difference quotients show that every derivative of order at least $k$ vanishes on $F\cap U$. Each polynomial component of $\Omega$ meeting $U$ has an endpoint in $F\cap U$, so its degree is less than $k$. Thus $f^{(k)}=0$ throughout $U$, contradicting $F\cap U\ne\varnothing$. Hence $\Omega=\mathbb R$, and its sole connected component carries one polynomial.

## ↑ Ancestors (8)

1. [Baire category theorem](baire-category-theorem.md)
2. [Complete metric space](complete-metric-space.md)
3. [Metric space](metric-space.md)
4. [Topological analysis](topological-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
