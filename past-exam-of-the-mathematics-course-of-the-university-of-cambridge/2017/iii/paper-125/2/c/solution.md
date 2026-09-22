<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $K^{\rm ur}$ be the [maximal unramified extension](../../../../../../maximal-unramified-extension.md) of $K$, with [residue field](../../../../../../residue-field.md) $\overline k$. First show that every geometric solution of $nQ=P$ lies in $E(K^{\rm ur})$.

The [multiplication-by-n morphism](../../../../../../multiplication-by-n-morphism.md) on the reduced [elliptic curve](../../../../../../elliptic-curve.md) is surjective over $\overline k$. Choose $\overline Q$ with $n\overline Q=\overline P$, defined over some finite [finite field extension](../../../../../../finite-field-extension.md) $k'/k$. Let $L/K$ be the corresponding finite [unramified extension](../../../../../../unramified-extension.md). By the [surjectivity of good reduction over a local field](../../../../../../surjectivity-of-good-reduction-over-a-local-field.md), lift $\overline Q$ to $Q_0\in E(L)$. Then $P-nQ_0\in E_1(L)$. The [multiplication isomorphism of a formal group law](../../../../../../multiplication-isomorphism-of-a-formal-group-law.md) gives a unique $R\in E_1(L)$ with $nR=P-nQ_0$, so $Q_0+R$ is an $n$-division point of $P$ defined over $L$.

Taking $P=O$ gives every element of $E[n]$ over $K^{\rm ur}$: reduction is injective on this [torsion point of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md) group because $[n]$ is injective on the formal kernel, and each reduced $n$-torsion point has the unique corrected lift just constructed. Every other division point differs from one lift by an element of $E[n]$. Hence the entire field $K([n]^{-1}P)$ is unramified, not merely a field containing one choice of $Q$.

To bound the composite uniformly in $P$, put $f=[K(E[n]):K]$. This [division field of an elliptic curve](../../../../../../division-field-of-an-elliptic-curve.md) is unramified. The [Galois group](../../../../../../galois-group.md) of $K^{\rm ur}/K$ is procyclic, generated topologically by its Frobenius element $\sigma$, and $\sigma^f$ fixes every element of $E[n]$. If $nQ=P\in E(K)$, then

$$
T=\sigma^fQ-Q\in E[n],\qquad \sigma^fT=T.
$$

Iteration gives $\sigma^{jf}Q=Q+jT$. In particular $\sigma^{nf}Q=Q$. Thus every such $Q$, for every $P$ together, lies in the unique [unramified extension](../../../../../../unramified-extension.md) of degree $nf$. If $M$ is the composite of all these fields, the [uniform unramified division field over a local field](../../../../../../uniform-unramified-division-field-over-a-local-field.md) gives

$$
\boxed{M/K\text{ is finite unramified},\qquad [M:K]\leq n[K(E[n]):K].}
$$

The prime-to-$p$ hypothesis is essential to the inverse-series argument; no assertion about arbitrary $p$-division is being made.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
