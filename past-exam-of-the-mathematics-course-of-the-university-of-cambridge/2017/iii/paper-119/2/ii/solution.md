<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $F$ is a [full and faithful functor](../../../../../../full-and-faithful-functor.md) and its essential image is closed under [strong quotients](../../../../../../strong-quotient.md). First its unit is invertible. To prove this directly, fullness gives $k:GFA\to A$ with $Fk=\varepsilon_{FA}$. The triangle identity and faithfulness give $k\eta_A=1_A$. [Naturality](../../../../../../naturality.md) of $\eta$ at $k$ and the other triangle identity give

$$
\eta_Ak=GFk\,\eta_{GFA}=G\varepsilon_{FA}\,\eta_{GFA}=1_{GFA}.
$$

Thus $\eta_A$ is an [isomorphism](../../../../../../isomorphism.md), and $\varepsilon_{FA}=(F\eta_A)^{-1}$ is also an [isomorphism](../../../../../../isomorphism.md).

Factor $\varepsilon_B$ as a [strong epimorphism](../../../../../../strong-epimorphism.md) followed by a [monomorphism](../../../../../../monomorphism.md). By closure under [strong quotients](../../../../../../strong-quotient.md), the intermediate object can, after transport along an [isomorphism](../../../../../../isomorphism.md), be written as $FA$:

$$
FGB\xrightarrow{e}FA\xrightarrow{m}B,\qquad \varepsilon_B=me.
$$

Fullness gives $e=Fk$ for $k:GB\to A$. Taking the transpose of $\varepsilon_B=mFk$ under the [adjunction](../../../../../../adjoint-functors.md), whose transpose is $1_{GB}$, gives

$$
1_{GB}=Gm\,GFk\,\eta_{GB}=Gm\,\eta_A\,k.
$$

Hence $k$ is a [split monomorphism](../../../../../../split-monomorphism.md), so $e=Fk$ is a [monomorphism](../../../../../../monomorphism.md). A [strong epimorphism](../../../../../../strong-epimorphism.md) which is monic is invertible: apply its lifting property to the square with that same map on both sides and identity top and bottom edges. Thus $e$ is invertible and $\varepsilon_B=me$ is monic. We have proved the [pointwise-monic unit-and-counit criterion](../../../../../../pointwise-monic-unit-and-counit-criterion.md):

$$
\boxed{\eta,\varepsilon\text{ monic}\iff F\text{ fully faithful with image closed under strong quotients}.}
$$

For a counterexample without the balanced hypothesis, use the [pointwise-monic adjunction over a non-balanced poset](../../../../../../pointwise-monic-adjunction-over-a-non-balanced-poset.md). Let $\mathcal C=\{0<1\}$ and let $\mathcal D$ have one object and only its identity. The unique $F:\mathcal C\to\mathcal D$ is left adjoint to $G$ selecting $1$, since both $\mathcal D(Fc,*)$ and $\mathcal C(c,1)$ are singletons. All [morphisms](../../../../../../morphism.md) in a [poset](../../../../../../partially-ordered-set.md) viewed as a [category](../../../../../../category-split.md) are [monomorphisms](../../../../../../monomorphism.md), so the unit and counit are monic. However $F$ is not full: the identity $F1\to F0$ has no preimage $1\to0$. The arrow $0\to1$ is both monic and epic but not invertible, so $\mathcal C$ is not a [balanced category](../../../../../../balanced-category.md). **The balanced hypothesis cannot be dropped.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
