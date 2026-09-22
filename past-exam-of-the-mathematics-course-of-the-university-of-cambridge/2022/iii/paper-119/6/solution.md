<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [semi-additive category](../../../../../semi-additive-category.md) is a category whose hom-sets are [commutative monoids](../../../../../commutative-monoid.md) and whose composition is additive in each variable, with finite products and coproducts.

Suppose first that $P=A\times B$ is a binary [product in a category](../../../../../product-category-theory.md), with projections $p_1,p_2$. The zero morphisms and the product property define maps

$$
i_1:A\to P,qquad i_2:B\to P
$$

by

$$
p_1i_1=1_A,quad p_2i_1=0,qquad
p_1i_2=0,quad p_2i_2=1_B.
$$

The two projections of $i_1p_1+i_2p_2$ equal those of $1_P$, so

$$
i_1p_1+i_2p_2=1_P.
$$

For $f:A\to C$ and $g:B\to C$, the map

$$
h=fp_1+gp_2:P\to C
$$

satisfies $hi_1=f$ and $hi_2=g$. If $k$ has the same restrictions, then

$$
k=k(i_1p_1+i_2p_2)=fp_1+gp_2=h.
$$

Thus $(P,i_1,i_2)$ is also the binary coproduct. The dual argument starts from a coproduct and makes it a product. Hence binary products and coproducts coincide canonically as [biproducts](../../../../../biproduct.md).

Let $f,g:A\rightrightarrows B$ be a [reflexive pair](../../../../../reflexive-pair.md) in an [additive category](../../../../../additive-category.md), with $fr=gr=1_B$. For every object $C$, regard $x:C\to A$ as an arrow from $fx$ to $gx$ between objects of $\mathcal C(C,B)$. The identity at $b:C\to B$ is $rb$.

If $gx=fy$, define the composite by

$$
x\circledast y=x+y-rgx.
$$

Its source and target are

$$
f(x\circledast y)=fx,qquad g(x\circledast y)=gy.
$$

The identities follow from

$$
rf x\circledast x=x,qquad x\circledast rgx=x,
$$

and associativity follows immediately by expanding both iterated composites and using the matching equations. The inverse of $x$ is

$$
x^{-1}=rfx+rgx-x,
$$

whose source is $gx$, whose target is $fx$, and whose two composites with $x$ are the appropriate identity arrows. These formulas are natural in $C$, so the [Yoneda lemma](../../../../../yoneda-lemma.md) identifies them with structure morphisms in $\mathcal C$. The pair is therefore an internal groupoid, proving that every [reflexive pair in an additive category is an internal groupoid](../../../../../reflexive-pair-in-an-additive-category-is-an-internal-groupoid.md).

This fails for semi-additive categories. In the category of [commutative monoids](../../../../../commutative-monoid.md), let

$$
R=\{(m,n)\in\mathbb N^2:m\leq n\}
$$

under coordinatewise addition. The two projections $f,g:R\rightrightarrows\mathbb N$ have the common splitting $r(n)=(n,n)$, so they form a reflexive pair. Its underlying reflexive graph is the usual order category on $\mathbb N$: there is an arrow $m\to n$ exactly when $m\leq n$. If it were an internal groupoid, the arrow $0\to1$ would have an inverse $1\to0$, but $(1,0)\notin R$. Therefore this reflexive pair is not an internal groupoid, and “additive” cannot be weakened to “semi-additive.”

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
