<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $q=p^n$. A finitely generated [module](../../../../../../module-mathematics.md) over $A=k[X]/(X^q)$ is finite-dimensional over $k$, and multiplication by $X$ is a [nilpotent linear map](../../../../../../nilpotent-linear-map.md) $T$ with $T^q=0$. Its [Jordan normal form](../../../../../../jordan-normal-form.md) exists over $k$ because its minimal polynomial is a power of $X$. Each [Jordan block](../../../../../../jordan-block.md) has size $r\le q$ and is the [cyclic module](../../../../../../cyclic-module.md) $M_r=k[X]/(X^r)$. Hence

$$
M\cong\bigoplus_{r=1}^{q}M_r^{\oplus m_r}.
$$

A [submodule](../../../../../../submodule.md) of $M_r$ is an ideal of $k[X]/(X^r)$, and its inverse image is an ideal of the [principal ideal domain](../../../../../../principal-ideal-domain.md) $k[X]$ containing $(X^r)$. The only possibilities are $(X^j)$ with $0\le j\le r$. Thus all [submodules](../../../../../../submodule.md) form the chain

$$
M_r\supset XM_r\supset\cdots\supset X^{r-1}M_r\supset0.
$$

Every successive quotient is the one-dimensional [simple module](../../../../../../irreducible-module.md) on which $X$ acts as zero. This is its unique [composition series](../../../../../../composition-series.md), so $M_r$ is a [uniserial module](../../../../../../uniserial-module.md) and is an [indecomposable representation](../../../../../../indecomposable-representation.md): two nonzero direct summands would be incomparable [submodules](../../../../../../submodule.md). Only $M_1$ is simple.

For $G=\langle g\rangle$ of order $q$, the [group algebra](../../../../../../group-algebra.md) satisfies

$$
kG\cong k[T]/(T^q-1)\cong k[X]/(X^q),\qquad X=g-1,
$$

since $(T-1)^q=T^q-1$ in [characteristic](../../../../../../characteristic-of-a-field.md) $p$. Consequently, up to isomorphism, $\boxed{M_1,\ldots,M_{p^n}}$ are precisely the finite-dimensional indecomposable modules, and $\boxed{M_1\text{ is the unique simple module}}$. The finite-dimensional convention follows from the finite-generation hypothesis; “exactly” counts isomorphism classes.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
