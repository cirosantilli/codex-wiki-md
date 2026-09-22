<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An [abelian category](../../../../../abelian-category.md) is an [additive category](../../../../../additive-category.md) with [kernels in a category](../../../../../kernel-in-a-category.md) and [cokernels in a category](../../../../../cokernel-in-a-category.md) in which the canonical comparison from [coimage](../../../../../coimage.md) to image of every morphism is an [isomorphism](../../../../../isomorphism.md). This is the standard image-coimage form of the definition, equivalently expressed by normality of every [monomorphism](../../../../../monomorphism.md) and [epimorphism](../../../../../epimorphism.md). Additivity means abelian-group hom-sets with bilinear composition, a [zero object](../../../../../zero-object.md) and finite [biproducts](../../../../../biproduct.md). A sequence is exact at an object when the image of the incoming morphism is the [kernel in a category](../../../../../kernel-in-a-category.md) of the outgoing one.

For $f:X\to Y$, construct $q:X\to\operatorname{coim}f=\operatorname{coker}(\ker f)$ and $j:\operatorname{im}f=\operatorname{ker}(\operatorname{coker}f)\to Y$. The [universal properties](../../../../../universal-property.md) give $f=j\bar f q$: first $f$ kills its [kernel in a category](../../../../../kernel-in-a-category.md) and factors through $q$; then the resulting map is killed by $\operatorname{coker}f$ because $q$ is epic, so it factors through $j$. The comparison $\bar f$ is invertible by the abelian axiom. [Cokernels in a category](../../../../../cokernel-in-a-category.md) are epic and [kernels in a category](../../../../../kernel-in-a-category.md) monic, directly by uniqueness in their [universal properties](../../../../../universal-property.md), so $e=\bar f q$ is epic and $j$ monic. Thus $\boxed{f=je\text{ is an epimorphism-monomorphism factorization}}$.

In a short exact sequence $0\to X\overset{i}{\to}Y\overset{p}{\to}Z\to0$, we have $i=\ker p$ and $p=\operatorname{coker}i$, up to the canonical [isomorphisms](../../../../../isomorphism.md). If $r:Y\to X$ retracts $i$, the map $1_Y-ir$ kills $i$ and factors as $sp$ for some $s:Z\to Y$. Composing with $p$ gives $psp=p$, so epicity gives $ps=1_Z$. Conversely if $ps=1_Z$, then $1_Y-sp$ is killed by $p$ and factors as $ir$. Composing with $i$ gives $iri=i$, so monicity gives $ri=1_X$. Consequently

$$
\boxed{i\text{ is split monic}\iff p\text{ is split epic}.}
$$

In that case $Y\cong X\oplus Z$.

For the derived-functor requests, use additive [right exact functors](../../../../../right-exact-additive-functor.md), as customary in abelian homological algebra. An [abelian category with enough projectives](../../../../../abelian-category-with-enough-projectives.md) permits an augmented [projective resolution](../../../../../projective-resolution.md) $\cdots\to P_2\to P_1\to P_0\to X\to0$, obtained by repeatedly taking an [epimorphism](../../../../../epimorphism.md) from a projective onto the previous [kernel in a category](../../../../../kernel-in-a-category.md). Apply $F$ and define

$$
L_nF(X)=H_n(FP_\bullet),\qquad L_0F(X)\cong F(X).
$$

Projective lifts construct maps of resolutions; the comparison and chain-homotopy results make the construction independent of choices and functorial. For a short exact sequence, the horseshoe construction produces a degreewise split short exact sequence of resolutions, hence of their images under additive $F$. Its [homology objects](../../../../../homology-object.md) give the long exact sequence

$$
\cdots\to L_2F(X)\to L_2F(Y)\to L_2F(Z)\to
L_1F(X)\to L_1F(Y)\to L_1F(Z)\to
F(X)\to F(Y)\to F(Z)\to0.
$$

This supplies the requested sketch; detailed comparison and functoriality proofs are not needed here.

A projective object $X$ has a resolution concentrated in degree zero, so $L_1F(X)=0$ for every such $F$. Conversely choose $0\to K\overset{i}{\to}P\to X\to0$ with $P$ projective, and take $F=\mathcal A(-,K)$ with target $\mathbf{Ab}^{\mathrm{op}}$. Precomposition makes this covariant to the [opposite category](../../../../../opposite-category.md). The usual left exactness of contravariant Hom, which follows directly from the [cokernel in a category](../../../../../cokernel-in-a-category.md) [universal property](../../../../../universal-property.md), says exactly that this $F$ is [right exact](../../../../../right-exact-additive-functor.md) in that opposite target. If $L_1F(X)=0$, the long exact sequence and $L_1F(P)=0$ make $F(K)\to F(P)$ monic in $\mathbf{Ab}^{\mathrm{op}}$. Equivalently,

$$
\operatorname{Hom}(P,K)\longrightarrow\operatorname{Hom}(K,K),\qquad r\longmapsto ri,
$$

is epic, hence surjective, in [abelian groups](../../../../../abelian-group.md). The identity of $K$ has a preimage, giving a retraction of $i$. The sequence splits, and $X$ is a [direct summand](../../../../../direct-summand.md) of $P$, hence projective: a lifting problem for $X$ extends along the projection $P\to X$, is solved for $P$, and restricts along the summand inclusion. Therefore

$$
\boxed{X\text{ projective}\iff L_1F(X)=0\text{ for every additive right exact }F.}
$$

This is [projectivity detected by all first left derived functors](../../../../../projectivity-detected-by-all-first-left-derived-functors.md). The following parts prove the three requested equivalent formulations of a [hereditary abelian category with enough projectives](../../../../../hereditary-abelian-category-with-enough-projectives.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
