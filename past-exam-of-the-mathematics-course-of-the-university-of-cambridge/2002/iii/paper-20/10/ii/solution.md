<h1 id="10/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the [free algebra functor](../../../../../../free-algebra-functor.md) $F^T$ by $F^T X=(TX,\mu_X)$ and $F^T f=Tf$. The [monad](../../../../../../monad.md) laws make $\mu_X$ an algebra action, and [naturality](../../../../../../naturality.md) of $\mu$ makes $Tf$ a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md). For an [algebra for a monad](../../../../../../algebra-for-a-monad.md) $(A,a)$, define

$$
\mathcal C^T(F^TX,(A,a))\longrightarrow\mathcal C(X,A),\quad h\longmapsto h\eta_X,
$$

with proposed inverse $g\mapsto aTg$. This inverse is a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md), since

$$
(aTg)\mu_X=a\mu_A T^2g=aTa\,T^2g=aT(aTg).
$$

One composite is $aTg\eta_X=a\eta_Ag=g$. For a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) $h$, the other is $aT(h\eta_X)=aTh\,T\eta_X=h\mu_X T\eta_X=h$. Both formulas commute with [composition in a category](../../../../../../composition-in-a-category.md) in $X$ and with [monad algebra morphisms](../../../../../../morphism-of-algebras-for-a-monad.md) in $(A,a)$, so the [bijection](../../../../../../bijection.md) is natural. Thus

$$
\boxed{F^T\dashv U.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10](../../10.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
