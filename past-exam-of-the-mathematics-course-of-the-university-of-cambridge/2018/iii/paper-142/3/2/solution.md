<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [K-theory transfer of a finite covering](../../../../../../k-theory-transfer-of-a-finite-covering.md), let $V\to Y$ be a [vector bundle](../../../../../../vector-bundle.md) and define

$$
(p_!V)_x=\bigoplus_{y\in p^{-1}(x)}V_y.
$$

On an evenly covered neighborhood the $n$ sheets identify this with a [direct sum](../../../../../../direct-sum.md) of $n$ local [vector bundles](../../../../../../vector-bundle.md). On overlaps the identifications permute the sheets and apply the transition maps of $V$, so these local descriptions glue to a [vector bundle](../../../../../../vector-bundle.md) on $X$. This operation respects [direct sums](../../../../../../direct-sum.md), hence extends to a homomorphism of [Grothendieck groups](../../../../../../grothendieck-group.md)

$$
\boxed{p_!:K^0(Y)\longrightarrow K^0(X),\qquad
p_!([V]-[W])=[p_!V]-[p_!W].}
$$

It obeys the [projection formula for the K-theory transfer](../../../../../../projection-formula-for-the-k-theory-transfer.md):

$$
p_!(p^*a\cdot b)=a\cdot p_!b.
$$

For actual [vector bundles](../../../../../../vector-bundle.md), this follows fiberwise by distributing the [tensor product of vector bundles](../../../../../../tensor-product-of-vector-bundles.md) over the [direct sum](../../../../../../direct-sum.md); it then extends to their [Grothendieck groups](../../../../../../grothendieck-group.md).

Let $P=p_!(1_Y)$ be the permutation [vector bundle](../../../../../../vector-bundle.md) of the covering. It has rank $n$ on every [connected component](../../../../../../connected-component.md), but need not be a [trivial vector bundle](../../../../../../trivial-vector-bundle.md); in particular one cannot replace $p_!p^*$ by multiplication by $n$ integrally. Instead write

$$
[P]=n+\eta,\qquad \eta\in I(X).
$$

The componentwise nilpotence result from the preceding solution gives $\eta^N=0$ for some $N$. In the [localization of a ring](../../../../../../localization-of-a-ring.md) $K^0(X)\otimes\mathbb Z[1/n]$, the finite [geometric series](../../../../../../geometric-series.md)

$$
(n+\eta)^{-1}=\frac1n\sum_{j=0}^{N-1}\left(-\frac{\eta}{n}\right)^j
$$

is an inverse. The [projection formula for the K-theory transfer](../../../../../../projection-formula-for-the-k-theory-transfer.md) gives

$$
p_!p^*(a)=[P]a=(n+\eta)a.
$$

Thus $p^*(a)=0$ implies $a=0$ after inverting $n$. More explicitly, $(n+\eta)^{-1}p_!$ is a left inverse, proving

$$
\boxed{p^*:K^0(X)\otimes\mathbb Z[1/n]\hookrightarrow K^0(Y)\otimes\mathbb Z[1/n].}
$$

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 142](../../../paper-142-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
