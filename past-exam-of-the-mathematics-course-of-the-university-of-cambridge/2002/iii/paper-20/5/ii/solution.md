<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Working with a [small category](../../../../../../small-category.md) $\mathcal C$ (or in a fixed ambient universe), for a [categorical presheaf](../../../../../../presheaf-category-theory.md) $X$ and fixed $U$, apply the [categorical coend](../../../../../../coend-of-a-functor.md) construction to $T(A,B)=\mathcal C(U,B)\times X(A)$. It is the quotient of the [disjoint union](../../../../../../disjoint-union.md) of pairs $(h:U\to W,x\in X(W))$ by the relations

$$
(fh,x)\sim(h,X(f)x)\qquad(f:W\to V,\ x\in X(V)).
$$

Define $\Phi_U([h,x])=X(h)x$. It respects every relation because $X(fh)x=X(h)X(f)x$. Define $\Psi_U(y)=[1_U,y]$. Then $\Phi_U\Psi_U(y)=y$. Conversely the relation with $f=h:U\to W$ gives $[h,x]=[1_U,X(h)x]$, so $\Psi_U\Phi_U$ is the [identity morphism](../../../../../../identity-morphism.md). Therefore

$$
\boxed{X(U)\cong\int^W\mathcal C(U,W)\times X(W).}
$$

For $k:V\to U$, restriction on the [categorical coend](../../../../../../coend-of-a-functor.md) sends $[h,x]$ to $[hk,x]$, and $\Phi_V([hk,x])=X(k)\Phi_U([h,x])$. A [natural transformation](../../../../../../natural-transformation.md) $X\to Y$ likewise acts on the second coordinate and commutes with $\Phi$. Thus the [density formula for presheaves](../../../../../../density-formula-for-presheaves.md) is a [natural isomorphism](../../../../../../natural-isomorphism.md), not just a family of unrelated [bijections](../../../../../../bijection.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
