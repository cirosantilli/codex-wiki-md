<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Work in ordinary set theory with the [axiom of choice](../../../../../axiom-of-choice.md). A [regular category](../../../../../regular-category.md) has [finite limits](../../../../../finite-limit.md), image factorizations as [regular epimorphisms](../../../../../regular-epimorphism.md) followed by [monomorphisms](../../../../../monomorphism.md), and pullback-stable regular epimorphisms. A [regular functor](../../../../../regular-functor.md) preserves finite limits and regular epimorphisms.

A [capital regular category](../../../../../capital-regular-category.md) is one whose [well-supported objects](../../../../../well-supported-object.md) are [well-pointed objects in a category](../../../../../well-pointed-object-in-a-category.md). Here well-supported means $A\to1$ is a regular epimorphism; well-pointed means a subobject of $A$ containing every point $1\to A$ must be the whole object. This is the convention of [Definition 1.3](https://www2.math.ethz.ch/EMIS/journals/TAC/volumes/16/31/16-31.pdf). It permits objects of proper support with no points. Replacing this condition by global points detecting every isomorphism would change the assertion: a three-element chain is regular but cannot admit a conservative finite-limit-preserving functor to such a category.

Here is a regular-logic proof sketch of [capitalization of a small regular category](../../../../../capitalization-of-a-small-regular-category.md). Use a sort for every object of $\mathcal C$, a function symbol for every morphism, and [regular theory](../../../../../regular-theory.md) axioms for composition, finite limiting diagrams and regular-epimorphism lifting. Its set models are precisely regular functors $\mathcal C\to\mathbf{Set}$. Empty sorts must be allowed.

The key separation lemma is the [regular-logic separation of a proper subobject](../../../../../regular-logic-separation-of-a-proper-subobject.md). For $m:S\hookrightarrow A$ proper, the sequent

$$
\top\ \vdash_{x:A}\ \exists y:S\ (m(y)=x)
$$

is not derivable: interpreting a derivation in $\mathcal C$ would make the monomorphism $m$ a regular epimorphism, hence an isomorphism. The [chase completeness for regular logic](../../../../../chase-completeness-for-regular-logic.md) supplies a set model in which it fails. Briefly, start with a named antecedent element, adjoin witnesses for the existential axioms, and quotient by required equalities. Every consequent about the original parameter arising at a finite stage has a finite proof; thus a nonderivable consequent remains false. The filtered union is the desired model. This witness construction, rather than an assumption that every sort is inhabited, is what keeps proper supports distinguishable.

Since $\mathcal C$ is small, choose a set-indexed family $(M_i)_{i\in I}$ of regular functors, one detecting each proper monomorphism, and form

$$
P:\mathcal C\longrightarrow\mathbf{Set}^{I},\qquad
P(A)=(M_iA)_{i\in I}.
$$

It is regular by coordinatewise finite limits and surjections. It reflects invertibility of monomorphisms. If $P(f)$ is invertible, apply this fact to the image inclusion of $f$ and to the diagonal of its [kernel pair](../../../../../kernel-pair.md). They are invertible, so $f$ is both a regular epimorphism and a monomorphism, hence invertible. Thus $P$ is a [conservative functor](../../../../../conservative-functor.md).

The target is a [power of sets as a capital regular category](../../../../../power-of-sets-as-a-capital-regular-category.md). A well-supported family has every coordinate nonempty, and choice extends any coordinate element to a global tuple. A subobject containing every tuple must consequently contain every coordinate element. Therefore it is capital, giving the required isomorphism-reflecting regular functor. This is the separation aspect of the regular representation results originating in [Barr's embedding work](https://math.mcgill.ca/barr/papers/embed.pdf); full faithfulness is unnecessary here.

The stronger target of a single set category has a precise restriction: **$\mathcal C$ admits a conservative regular functor to the [Category of sets](../../../../../category-of-sets.md) exactly when it is an [almost totally supported regular category](../../../../../almost-total-support-for-a-regular-category.md).** This means every object is well-supported or a [strict initial object](../../../../../strict-initial-object.md). Here are necessity and sufficiency.

Suppose $V:\mathcal C\to\mathbf{Set}$ is regular and conservative. If $VA$ is nonempty, its support in sets is $1$. Since $V$ preserves images, it sends the support inclusion $\sigma(A)\hookrightarrow1$ to an isomorphism; conservativity makes $\sigma(A)=1$, so $A$ is well-supported.

If $VA$ is empty, every projection $A\times X\to A$ is sent to the unique bijection between empty sets, hence is invertible. This supplies a morphism $A\to X$ for every $X$. The equalizer of any two such morphisms is also sent to a bijection, hence is invertible, proving uniqueness. Thus $A$ is initial. Every arrow $Y\to A$ forces $VY$ to be empty and is then sent to a bijection; conservativity makes it invertible. So $A$ is strict initial.

Conversely suppose this support condition holds. Use $P$ above and take

$$
V(A)=\prod_{i\in I}M_i(A).
$$

Products preserve finite limits and, by choice, coordinatewise surjections, so $V$ is regular. A well-supported object has all coordinates nonempty. A proper strict initial object has a subterminal image in every coordinate, with at least one empty coordinate: otherwise its arrow to $1$ would be sent by $P$ to an isomorphism, contradicting conservativity.

If $Vf$ is a bijection between well-supported objects, the [conservativity of set products on totally supported families](../../../../../conservativity-of-set-products-on-totally-supported-families.md) makes each $M_i(f)$ bijective: a missing coordinate preimage or a pair of equal-image coordinate elements extends to a tuple witnessing failure of surjectivity or injectivity. Hence $P(f)$ is invertible and so is $f$. An arrow between strict initial objects is already invertible; an arrow from a strict initial object to a well-supported object cannot become a bijection between empty and nonempty sets. An arrow into a strict initial object is invertible by definition. These cases prove conservativity and the [conservative regular representation in sets](../../../../../conservative-regular-representation-in-sets.md) criterion.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [Section B](../section-b.md)
3. [Paper 23](../../paper-23-split.md)
4. [Iii](../../split.md)
5. [2004](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
