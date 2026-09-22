<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Necessity follows from commutativity of the [fibre product of schemes](../../../../../../fiber-product-of-schemes.md) square: if $p(z)=x$ and $q(z)=y$, then $f(x)=g(y)$.

For sufficiency, put $s=f(x)=g(y)$ and $K=\kappa(s)$, $L=\kappa(x)$, $L'=\kappa(y)$. The maps on [local rings](../../../../../../local-ring.md) induce field embeddings $K\hookrightarrow L,L'$. The canonical point maps into $X$ and $Y$ therefore give a [morphism of schemes](../../../../../../morphism-of-schemes.md)

$$
\operatorname{Spec}(L\otimes_KL')
=\operatorname{Spec}L\times_{\operatorname{Spec}K}\operatorname{Spec}L'
\longrightarrow X\times_SY.
$$

The [tensor product of commutative algebras](../../../../../../tensor-product-of-commutative-algebras.md) $L\otimes_KL'$ is nonzero. To see the hinted fact directly, choose a $K$-basis of $L$ containing $1$; tensoring that basis with $L'$ makes $1\otimes1$ nonzero. A nonzero unital [commutative ring](../../../../../../commutative-ring.md) has a [prime ideal](../../../../../../prime-ideal.md), so its [spectrum of a commutative ring](../../../../../../spectrum-of-a-commutative-ring.md) has a point $w$. Its projections to the two field spectra are their unique points. The image $z$ of $w$ consequently projects to $x$ and $y$.

**The desired point exists precisely when the base images coincide.** This is the [point-lifting property of a scheme fibre product](../../../../../../point-lifting-property-of-a-scheme-fibre-product.md). It does not claim that such a point is unique: different [prime ideals](../../../../../../prime-ideal.md) of the tensor product may give different points over the same pair.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
