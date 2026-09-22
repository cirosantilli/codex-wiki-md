<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $A=k[X]$. There is an explicit [isomorphism](../../../../../../isomorphism.md) from the [principal open subset](../../../../../../principal-open-subscheme.md) $U_f$ to the [affine algebraic set](../../../../../../affine-algebraic-set.md)

$$
Z=V(sf-1)\subset X\times\mathbb A^1,\qquad x\longmapsto(x,f(x)^{-1}).
$$

Its inverse is projection, and both maps are [regular maps](../../../../../../morphism-of-algebraic-varieties.md). The [coordinate ring](../../../../../../coordinate-ring.md) is

$$
k[Z]=A[s]/(sf-1)\cong A_f,
$$

by the [universal property of localization](../../../../../../universal-property-of-localization.md). Since [regular functions](../../../../../../regular-function.md) on an [affine variety](../../../../../../affine-algebraic-set.md) are its [coordinate ring](../../../../../../coordinate-ring.md), this proves the natural $k$-[algebra isomorphism](../../../../../../algebra-isomorphism.md)

$$
\boxed{k[U_f]\cong k[X]_f.}
$$

Now $W=D(x)\cup D(y)$. A [regular function](../../../../../../regular-function.md) on $W$ determines one element of the [function field](../../../../../../function-field-of-an-algebraic-variety.md) $k(x,y)$, and its restrictions belong to $k[x,y]_x$ and $k[x,y]_y$. Conversely, elements of their intersection glue because they agree on $D(xy)$. Thus

$$
k[W]=k[x,y]_x\cap k[x,y]_y\subset k(x,y).
$$

If a reduced fraction has denominator dividing a power of $x$ and also a power of $y$, [unique factorization](../../../../../../unique-factorization-in-an-integral-domain.md) makes its denominator a [unit](../../../../../../unit-in-a-ring.md). Therefore **puncturing the plane does not change its ring of global [regular functions](../../../../../../regular-function.md)**:

$$
\boxed{k[W]=k[x,y].}
$$

If $W$ were an [affine variety](../../../../../../affine-algebraic-set.md), its inclusion $j:W\hookrightarrow\mathbb A^2$ would correspond to the identity [isomorphism](../../../../../../isomorphism.md) $k[x,y]\to k[W]$. The equivalence between [affine varieties](../../../../../../affine-algebraic-set.md) and their [coordinate rings](../../../../../../coordinate-ring.md) would make $j$ an [isomorphism](../../../../../../isomorphism.md), contradicting the missing origin. Hence **$W$ is not affine**. This illustrates [regular functions on the punctured affine plane](../../../../../../regular-functions-on-the-punctured-affine-plane.md): the [coordinate ring](../../../../../../coordinate-ring.md) alone does not recover a nonaffine [variety](../../../../../../algebraic-variety.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
