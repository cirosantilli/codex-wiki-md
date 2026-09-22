<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The [affine-target adjunction for schemes](../../../../../../affine-target-adjunction-for-schemes.md) gives the natural bijection**

$$
\boxed{\operatorname{Hom}_{\mathrm{Sch}}(X,\operatorname{Spec}A)
\simeq\operatorname{Hom}_{\mathrm{Ring}}(A,\Gamma(X,\mathcal O_X)).}
$$

A [morphism of schemes](../../../../../../morphism-of-schemes.md) $f$ gives the homomorphism on [global sections](../../../../../../global-section.md) induced by $f^\#$, using $\Gamma(\operatorname{Spec}A,\mathcal O)=A$.

Conversely, let $\alpha:A\to\Gamma(X,\mathcal O_X)$ be a [ring homomorphism](../../../../../../ring-homomorphism.md). Choose an [affine open subscheme](../../../../../../affine-open-subscheme.md) cover $U_i=\operatorname{Spec}B_i$ of $X$. Restriction of [global sections](../../../../../../global-section.md) gives homomorphisms $A\to B_i$, hence [morphisms of schemes](../../../../../../morphism-of-schemes.md) $f_i:U_i\to\operatorname{Spec}A$. On any [affine open subscheme](../../../../../../affine-open-subscheme.md) $W\subseteq U_i\cap U_j$, both restrictions correspond to the same homomorphism $A\to\Gamma(W,\mathcal O_W)$. They therefore agree on $W$. Such affine opens cover the overlap, so the $f_i$ glue uniquely to a [morphism of schemes](../../../../../../morphism-of-schemes.md) $f:X\to\operatorname{Spec}A$.

The two constructions are inverse: the first recovers $\alpha$ on each $U_i$, hence on all of $X$, and the second recovers every restriction $f|_{U_i}$ of a given $f$. This proof needs neither affineness nor [quasi-compactness](../../../../../../compact-space.md) of $X$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
