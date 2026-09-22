<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $m=\dim M$, $n=\dim N$ and $k=\operatorname{codim}_N S$. Fix $p\in f^{-1}(S)$ and choose the allowed [slice chart for an embedded submanifold](../../../../../../slice-chart-for-an-embedded-submanifold.md) on a neighborhood $U$ of $f(p)$, so that $S\cap U$ is given by $x^1=\cdots=x^k=0$. On $f^{-1}(U)$ define the [smooth map](../../../../../../smooth-map-between-manifolds.md)

$$
G=(x^1,\ldots,x^k)\circ f:f^{-1}(U)\longrightarrow\mathbb R^k.
$$

The derivative $L=d(x^1,\ldots,x^k)$ at a point of $S\cap U$ is surjective and has kernel $T S$, by the slice description. The printed sum-of-spaces condition gives

$$
L\bigl(df_r(T_rM)\bigr)=\mathbb R^k\qquad
\text{for every }r\in f^{-1}(S\cap U).
$$

Indeed any target tangent vector is a sum of an image vector and a tangent vector to $S$, and $L$ kills the latter. By the [chain rule](../../../../../../chain-rule.md), $dG_r=L\circ df_r$ is therefore surjective. This condition is precisely [transversality of a map to a submanifold](../../../../../../transversality-of-a-map-to-a-submanifold.md); the original sum need not be direct.

We have $G^{-1}(0)=f^{-1}(S)\cap f^{-1}(U)$. Part (b), applied to $G$, gives [slice charts for an embedded submanifold](../../../../../../slice-chart-for-an-embedded-submanifold.md) of codimension $k$ around every point of this zero set. Since the construction is available around every $p\in f^{-1}(S)$, the charts give its global structure as an [embedded submanifold](../../../../../../embedded-submanifold.md) with the [subspace topology](../../../../../../subspace-topology.md). **Its dimension is $\boxed{m-k=m-n+\dim S}$**. Moreover,

$$
\boxed{T_p(f^{-1}(S))=\{v\in T_pM:df_p(v)\in T_{f(p)}S\}.}
$$

This follows either from the slice coordinates or from $T_pG^{-1}(0)=\ker dG_p$ and $\ker L=T_{f(p)}S$. No injectivity of $df$, closedness of $S$, or direct-sum hypothesis is required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
