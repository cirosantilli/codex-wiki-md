<h1 id="22f/solution">Solution</h1>

↑ **Parent:** [22F](../22f.md)

A linear operator between Banach spaces is a [compact operator](../../../../../compact-operator-split.md) when it maps the [unit ball](../../../../../unit-ball.md) into a relatively [compact set](../../../../../compact-space.md), equivalently when every bounded sequence of inputs has an image subsequence converging in [norm](../../../../../norm.md). Such an operator is bounded. For a [bounded linear operator](../../../../../continuous-linear-operator.md) on a complex [Banach space](../../../../../banach-space-split.md), the [resolvent set](../../../../../resolvent-set-of-an-operator.md) consists of the complex $\lambda$ for which $T-\lambda I$ is bijective with bounded inverse; its complement is the [spectrum](../../../../../spectrum-functional-analysis.md). The [point spectrum](../../../../../point-spectrum.md) consists of those $\lambda$ for which $T-\lambda I$ has a nonzero [kernel](../../../../../kernel-of-a-linear-map.md), namely the [eigenvalues](../../../../../eigenvalue.md).

On a [Hilbert space](../../../../../hilbert-space-split.md), $T$ is [self-adjoint](../../../../../self-adjoint-operator.md) if $T=T^*$, or equivalently $\langle Tx,y\rangle=\langle x,Ty\rangle$ for all vectors. The given prescription extends uniquely to

$$
Tx=\sum_{j\geq1}\frac{x_j}{j}e_j,\qquad x=\sum_jx_je_j.
$$

It is bounded with [norm](../../../../../norm.md) one. The real diagonal entries prove self-adjointness by the inner-product identity. Define the finite-rank truncation $T_mx=\sum_{j\leq m}x_je_j/j$. Then $\|T-T_m\|=1/(m+1)\to0$. To see compactness directly, extract successively convergent subsequences of the finitely many first coordinates from a bounded input sequence; the uniform tail bound just displayed makes the resulting image subsequence Cauchy. Hence **$T$ is compact and [self-adjoint](../../../../../self-adjoint-operator.md)**.

Each $1/j$ is an [eigenvalue](../../../../../eigenvalue.md) with [eigenspace](../../../../../eigenspace.md) $\mathbb Ce_j$. If $Tx=\lambda x$, each coordinate satisfies $(1/j-\lambda)x_j=0$, so there are no other [eigenvalues](../../../../../eigenvalue.md); in particular zero is not an [eigenvalue](../../../../../eigenvalue.md). But $\|Te_j\|=1/j\to0$, which contradicts a bounded inverse at zero. Thus zero is in the [spectrum](../../../../../spectrum-functional-analysis.md).

For $\lambda\notin\{0,1,1/2,1/3,\ldots\}$, its distance from this [closed set](../../../../../closed-set.md) is positive. The diagonal formula

$$
(T-\lambda I)^{-1}y=\sum_{j\geq1}\frac{y_j}{1/j-\lambda}e_j
$$

then defines a bounded inverse. This proves the complete description

$$
\boxed{\sigma(T)=\{0\}\cup\{1/j:j\geq1\},\quad
\sigma_p(T)=\{1/j:j\geq1\},\quad
\rho(T)=\mathbb C\setminus\sigma(T).}
$$

## ↑ Ancestors (10)

1. [22F](../22f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
