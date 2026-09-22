<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [balanced category](../../../../../balanced-category.md) is one in which every morphism that is both a [monomorphism](../../../../../monomorphism.md) and an [epimorphism](../../../../../epimorphism.md) is an isomorphism. A [faithful functor](../../../../../faithful-functor.md) reflects monomorphisms and epimorphisms: cancellation after applying the functor can be pulled back by injectivity on hom-sets. Therefore, if $F:\mathcal C\to\mathcal D$ is faithful, $\mathcal C$ is balanced, and $F(f)$ is an isomorphism, then $f$ is both monic and epic and hence is an isomorphism. Thus $F$ reflects isomorphisms.

Now let $F:\mathcal C\rightleftarrows\mathcal D:G$ be an [adjunction](../../../../../adjoint-functors.md) with unit $\eta$ and counit $\varepsilon$. Under the adjunction bijection

$$
\mathcal D(FX,FA)\cong\mathcal C(X,GFA),
$$

the morphism $Fu$ corresponds to $\eta_Au$. If $F$ is faithful and $\eta_Au=\eta_Av$, then $Fu=Fv$ and hence $u=v$, so every $\eta_A$ is monic. Conversely, if every $\eta_B$ is monic and $Fu=Fv$ for $u,v:A\to B$, naturality gives

$$
\eta_Bu=GF(u)\eta_A=GF(v)\eta_A=\eta_Bv,
$$

and monicity gives $u=v$. This proves the [faithful left adjoint criterion](../../../../../faithful-left-adjoint-criterion.md).

Assume next that $\mathcal C$ is balanced, every arrow in $\mathcal D$ factors as a [strong epimorphism](../../../../../strong-epimorphism.md) followed by a monomorphism, and both $\eta$ and $\varepsilon$ are pointwise monic. The unit criterion makes $F$ faithful. The triangle identity

$$
\varepsilon_{FA}F(\eta_A)=1_{FA}
$$

makes the monomorphism $\varepsilon_{FA}$ a split epimorphism, hence an isomorphism. Thus $F(\eta_A)$ is an isomorphism. The first paragraph shows that $F$ reflects isomorphisms, so $\eta_A$ is an isomorphism for every $A$. By the [fully faithful adjoint criterion](../../../../../fully-faithful-adjoint-criterion.md), $F$ is full and faithful.

To prove closure under [strong quotients](../../../../../strong-quotient.md), let $q:FA\twoheadrightarrow B$ be a strong epimorphism. Naturality gives

$$
\varepsilon_BFG(q)=q\varepsilon_{FA}.
$$

The right side is a strong epimorphism, while $\varepsilon_B$ is monic. The lifting property supplies $s:B\to FGB$ with

$$
\varepsilon_Bs=1_B.
$$

Since $\varepsilon_B$ is also monic, it is an isomorphism. Hence $B\cong F(GB)$ lies in the essential image of $F$.

Conversely, assume $F$ is full and faithful and its image is closed under strong quotients. Then $\eta$ is an isomorphism and in particular pointwise monic. Factor a counit component as

$$
FGB\xrightarrow{e}C\xrightarrow{m}B,
$$

with $e$ strong epic and $m$ monic. Closure under strong quotients gives $C\cong FA'$ for some $A'$. After choosing this isomorphism, fullness writes $e=Fh$ for a map $h:GB\to A'$. Since $e$ is epic and $F$ is faithful, $h$ is epic. The transpose of

$$
\varepsilon_B=mFh
$$

is $1_{GB}$, so

$$
G(m)\eta_{A'}h=1_{GB}.
$$

Thus $h$ is also monic. Balancedness makes $h$ an isomorphism, hence $e$ is an isomorphism and $\varepsilon_B=m e$ is monic. This proves the [pointwise-monic unit-and-counit criterion](../../../../../pointwise-monic-unit-and-counit-criterion.md).

Balancedness is necessary. Let $\mathcal C$ be the two-element poset $0<1$, viewed as a category, and let $\mathcal D$ be the terminal category. The unique $F:\mathcal C\to\mathcal D$ is left adjoint to the functor $G$ selecting $1$. Every morphism in a poset is monic, so the unit and counit are pointwise monic. But $F$ is not full: the unique arrow $F1\to F0$ has no preimage $1\to0$. This is the [pointwise-monic adjunction over a non-balanced poset](../../../../../pointwise-monic-adjunction-over-a-non-balanced-poset.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
