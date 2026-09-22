<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [equivalence of categories](../../../../../equivalence-of-categories.md) consists of [functors](../../../../../functor.md) $F:\mathcal C\to\mathcal D$ and $G:\mathcal D\to\mathcal C$ together with invertible [natural transformations](../../../../../natural-transformation.md) $GF\cong1_{\mathcal C}$ and $FG\cong1_{\mathcal D}$. A strict [isomorphism of categories](../../../../../isomorphism-of-categories.md) instead requires a [functor](../../../../../functor.md) with an inverse whose composites are literally identity [functors](../../../../../functor.md).

First suppose $F$ belongs to an [equivalence of categories](../../../../../equivalence-of-categories.md). The isomorphisms $FGD\cong D$ give [essential surjectivity](../../../../../essential-surjectivity.md). If $Ff=Fg$, apply $G$ and conjugate by $GF\cong1_{\mathcal C}$ to obtain $f=g$, so $F$ is a [faithful functor](../../../../../faithful-functor.md). Similarly $G$ is a [faithful functor](../../../../../faithful-functor.md). Writing $\alpha:GF\xrightarrow{\sim}1_{\mathcal C}$, any $h:FA\to FB$ has a preimage

$$
f=\alpha_B\,G(h)\,\alpha_A^{-1}.
$$

Indeed [naturality](../../../../../naturality.md) of $\alpha$ gives $GF(f)=G(h)$, and faithfulness of $G$ gives $F(f)=h$. Thus $F$ is a [full and faithful functor](../../../../../full-and-faithful-functor.md).

Conversely, assume $F$ is a [full and faithful functor](../../../../../full-and-faithful-functor.md) and has [essential surjectivity](../../../../../essential-surjectivity.md). Using the [axiom of choice](../../../../../axiom-of-choice.md), for each $D$ choose an object $GD$ and an isomorphism $\theta_D:F(GD)\to D$. Define $G$ on a [morphism](../../../../../morphism.md) $h:D\to E$ by the unique lift

$$
F(Gh)=\theta_E^{-1}h\theta_D.
$$

The [full and faithful functor](../../../../../full-and-faithful-functor.md) property makes $G$ preserve identities and composition, and makes $\theta:FG\cong1_{\mathcal D}$ a [natural transformation](../../../../../natural-transformation.md). For $A\in\mathcal C$, lift $\theta_{FA}:FGFA\to FA$ uniquely to $\alpha_A:GFA\to A$. Lifting its inverse shows that $\alpha_A$ is invertible. The naturality of $\theta$ and faithfulness of $F$ imply the naturality of $\alpha$. This proves

$$
\boxed{F\text{ is an equivalence}\iff F\text{ is full, faithful and essentially surjective}.}
$$

For large [categories](../../../../../category-split.md), this choice argument is understood in a fixed universe, or with the corresponding class-choice convention; ordinary set-sized [axiom of choice](../../../../../axiom-of-choice.md) suffices for [small categories](../../../../../small-category.md).

For the [category of partial functions](../../../../../category-of-partial-functions.md), let $X_+=X\amalg\{*\}$, with a tagged new element as basepoint. Send a [partial function](../../../../../partial-function.md) $f:X\rightharpoonup Y$ to the basepoint-preserving total [function](../../../../../function-split.md)

$$
f_+(x)=\begin{cases}f(x),&x\in\operatorname{dom}f,\\ *,&x\notin\operatorname{dom}f,\end{cases}
\qquad f_+(*)=*.
$$

Undefined composition is sent to the basepoint, so this is a [functor](../../../../../functor.md) $(-)_+:\mathbf{Part}\to\mathbf{Set}_*$. Restriction away from the basepoint recovers each [partial function](../../../../../partial-function.md) uniquely; hence it is a [full and faithful functor](../../../../../full-and-faithful-functor.md). Every [pointed set](../../../../../pointed-set.md) $(Y,y_0)$ is isomorphic to $(Y\setminus\{y_0\})_+$, so there is an [equivalence of categories](../../../../../equivalence-of-categories.md). This particular equivalence can also be constructed explicitly, without choice, by deleting and adjoining the basepoint.

These actual [categories](../../../../../category-split.md) are **equivalent but not isomorphic**. In $\mathbf{Part}$ the empty [set](../../../../../set-split.md) is the only [zero object](../../../../../zero-object.md): if $X$ is nonempty, its identity differs from its nowhere-defined endomorphism, so it cannot be initial or terminal. In $\mathbf{Set}_*$ every singleton [pointed set](../../../../../pointed-set.md) is a [zero object](../../../../../zero-object.md), and distinct singleton underlying [sets](../../../../../set-split.md) give distinct objects. An [isomorphism of categories](../../../../../isomorphism-of-categories.md) is a bijection on objects preserving [zero objects](../../../../../zero-object.md); it cannot take one such object onto several. This uses the categories of all actual [sets](../../../../../set-split.md), as in the paper, rather than chosen [skeletal categories](../../../../../skeletal-category.md) of representatives.

A [skeletal category](../../../../../skeletal-category.md) has no distinct isomorphic objects. If an equivalence $F:\mathcal C\to\mathcal D$ joins two [skeletal categories](../../../../../skeletal-category.md), [essential surjectivity](../../../../../essential-surjectivity.md) becomes surjectivity on objects. If $FA=FB$, lift the identity of that object and its inverse using [full and faithful](../../../../../full-and-faithful-functor.md) to obtain $A\cong B$, so $A=B$. Thus $F$ is bijective on objects and on every hom-set. Its inverse on objects and [morphisms](../../../../../morphism.md) is a strictly inverse [functor](../../../../../functor.md), proving that it is an [isomorphism of categories](../../../../../isomorphism-of-categories.md).

Under the [axiom of choice](../../../../../axiom-of-choice.md), choose one object from each isomorphism class of a [small category](../../../../../small-category.md). The full [subcategory](../../../../../subcategory.md) on those objects is a [skeleton of a category](../../../../../skeleton-of-a-category.md), and its inclusion is a [full and faithful functor](../../../../../full-and-faithful-functor.md) with [essential surjectivity](../../../../../essential-surjectivity.md), hence an [equivalence of categories](../../../../../equivalence-of-categories.md).

For the converse, form the [small category](../../../../../small-category.md) which is a [groupoid](../../../../../groupoid.md) with objects $(i,a)$ for $a\in A_i$, and exactly one [morphism](../../../../../morphism.md) $(i,a)\to(j,b)$ when $i=j$, with no [morphisms](../../../../../morphism.md) when $i\ne j$. Suppose it is equivalent to a [skeletal category](../../../../../skeletal-category.md) $\mathcal S$, with quasi-inverse [functors](../../../../../functor.md) $H:\mathcal C\to\mathcal S$ and $K:\mathcal S\to\mathcal C$. For each $i$, the objects $H(i,a)$ for $a\in A_i$ are isomorphic, hence all equal to a uniquely determined $s_i$. The isomorphism $KH(i,a)\cong(i,a)$ ensures that $K(s_i)=(i,a_i)$ for some $a_i\in A_i$. The rule $i\mapsto a_i$ is a choice function. In particular, no representative in $A_i$ had to be chosen to define $s_i$, since it is unique. Consequently

$$
\boxed{\text{Every small category has a skeletal equivalent}\iff\text{the axiom of choice}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
