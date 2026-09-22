<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work on [affine open subsets](../../../../../../affine-open-subscheme.md). Their [coordinate rings](../../../../../../coordinate-ring.md) are [Noetherian rings](../../../../../../noetherian-ring.md) and [integrally closed domains](../../../../../../integrally-closed-domain.md). At a [prime ideal](../../../../../../prime-ideal.md) of [height of a prime ideal](../../../../../../height-of-a-prime-ideal.md) one, the [local ring](../../../../../../local-ring.md) is a one-dimensional [Noetherian local ring](../../../../../../noetherian-local-ring.md) which is an [integrally closed domain](../../../../../../integrally-closed-domain.md), hence a [discrete valuation ring](../../../../../../discrete-valuation-ring.md) and therefore a [regular local ring](../../../../../../regular-local-ring.md). At the generic point the [local ring](../../../../../../local-ring.md) is a [field](../../../../../../field.md), hence a [regular local ring](../../../../../../regular-local-ring.md). For a brief justification of the one-dimensional [local ring](../../../../../../local-ring.md) fact, take $0\ne a\in\mathfrak m$ in a one-dimensional [Noetherian local ring](../../../../../../noetherian-local-ring.md) $R$ which is an [integrally closed domain](../../../../../../integrally-closed-domain.md). Some $\mathfrak m^n\subset(a)$; choose the least such $n$, and choose $b\in\mathfrak m^{n-1}\setminus(a)$. Then $q=b/a\notin R$, but $q\mathfrak m\subset R$. If $q\mathfrak m\subset\mathfrak m$, the [determinant trick](../../../../../../determinant-trick.md) applied to the finitely generated faithful module $\mathfrak m$ would make $q$ integral over $R$, a contradiction. Hence the ideal $q\mathfrak m$ contains a unit and equals $R$. Thus $\mathfrak m=q^{-1}R$ is principal. A one-dimensional [Noetherian local ring](../../../../../../noetherian-local-ring.md) with principal maximal ideal is a [discrete valuation ring](../../../../../../discrete-valuation-ring.md). Therefore a [normal variety](../../../../../../normal-variety.md) is [regular in codimension one](../../../../../../regular-in-codimension-one.md).

The ground [field](../../../../../../field.md) is an [algebraically closed field](../../../../../../algebraically-closed-field.md), hence a [perfect field](../../../../../../perfect-field.md), so having a [regular local ring](../../../../../../regular-local-ring.md) is equivalent to being a [smooth point of a variety](../../../../../../smooth-point-of-a-variety.md) here. Moreover, the [smooth locus of a variety](../../../../../../smooth-locus-of-a-variety.md) is open, making the [singular locus](../../../../../../singular-locus.md) closed. If an [irreducible component](../../../../../../irreducible-component.md) of the [singular locus](../../../../../../singular-locus.md) had [algebraic codimension](../../../../../../codimension-of-an-algebraic-subvariety.md) zero or one, its generic point would have a [regular local ring](../../../../../../regular-local-ring.md) by the preceding argument, a contradiction. Consequently every such component has [algebraic codimension](../../../../../../codimension-of-an-algebraic-subvariety.md) at least two.

One can read the numerical bound directly from chains of [prime ideals](../../../../../../prime-ideal.md), without identifying [algebraic dimension](../../../../../../dimension-of-an-algebraic-set.md) with [transcendence degree](../../../../../../transcendence-degree.md). For a [prime ideal](../../../../../../prime-ideal.md) $P$ of [height of a prime ideal](../../../../../../height-of-a-prime-ideal.md) at least two in an [affine chart](../../../../../../affine-chart-of-a-variety.md), append a chain $(0)\subsetneq P_1\subsetneq P$ below any chain in the quotient by $P$. Its length increases by two. Thus $\dim A/P\le\dim A-2$. Since a nonempty [affine open subset](../../../../../../affine-open-subscheme.md) of the [irreducible variety](../../../../../../irreducible-variety.md) $X$ has [algebraic dimension](../../../../../../dimension-of-an-algebraic-set.md) $d$,

$$
\boxed{\dim\operatorname{Sing}(X)\le d-2.}
$$

For $d=0$ or $1$, this means the [singular locus](../../../../../../singular-locus.md) is empty; take $\dim\varnothing=-\infty$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
