<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [categorical presheaf](../../../../../../presheaf-category-theory.md) $X$, its [category of elements](../../../../../../category-of-elements.md) has objects $(C,x)$ with $x\in X(C)$. A [morphism](../../../../../../morphism.md) $(C,x)\to(D,y)$ is a [morphism](../../../../../../morphism.md) $f:C\to D$ satisfying $X(f)(y)=x$. [Composition in a category](../../../../../../composition-in-a-category.md) is inherited from $\mathcal C$: if also $X(g)(z)=y$, then $X(gf)(z)=X(f)X(g)(z)=x$. The [identity morphisms](../../../../../../identity-morphism.md) are inherited as well. The [forgetful functor](../../../../../../forgetful-functor.md) sends $(C,x)$ to $C$ and $f$ to $f$.

A [universal element](../../../../../../universal-element-of-a-set-valued-functor.md) is a pair $(R,r)$ for which each $x\in X(C)$ is uniquely of the form $X(f)(r)$ for $f:C\to R$. Thus $(R,r)$ is a [terminal object](../../../../../../terminal-object.md) of the [category of elements](../../../../../../category-of-elements.md), with the variance appropriate to a [categorical presheaf](../../../../../../presheaf-category-theory.md).

Given a [universal element](../../../../../../universal-element-of-a-set-valued-functor.md), define

$$
\psi_C:\mathcal C(C,R)\longrightarrow X(C),\qquad f\longmapsto X(f)(r).
$$

The defining uniqueness makes each map a [bijection](../../../../../../bijection.md); $X(u)\psi_C(f)=\psi_{C'}(fu)$ gives [naturality](../../../../../../naturality.md) for $u:C'\to C$. Hence $\psi$ is a [natural isomorphism](../../../../../../natural-isomorphism.md) and $X$ is a [representable presheaf](../../../../../../representable-functor.md). Conversely, from a [natural isomorphism](../../../../../../natural-isomorphism.md) $\psi:\mathcal C(-,R)\cong X$, take $r=\psi_R(1_R)$. The [Yoneda lemma](../../../../../../yoneda-lemma.md) gives $\psi_C(f)=X(f)(r)$; its bijectivity makes $(R,r)$ a [universal element](../../../../../../universal-element-of-a-set-valued-functor.md). Therefore **the two descriptions coincide**:

$$
\boxed{X\text{ is representable}\iff\operatorname{Elts}(X)\text{ has a terminal object}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
