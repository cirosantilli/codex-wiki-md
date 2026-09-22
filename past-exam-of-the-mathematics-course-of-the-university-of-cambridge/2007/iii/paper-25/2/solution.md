<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Definitions organize [category theory](../../../../../category-theory-split.md), but theorems give that organization mathematical force.** I would therefore argue against treating the subject as an exception in which definitions are intrinsically more important than theorems. The distinction is especially misleading here because good categorical definitions are designed to expose hypotheses from which substantial theorems follow.

A [category](../../../../../category-split.md) records objects, composable arrows, identities and associative composition. A [functor](../../../../../functor.md) preserves that structure. This language allows one to compare otherwise different mathematical settings, but it does not itself say which constructions exist. For example, the definition of a [product in a category](../../../../../product-category-theory.md) is not a recipe for forming a [Cartesian product](../../../../../cartesian-product.md) of underlying sets: it requires a universal factorization of pairs of arrows. If two [products in a category](../../../../../product-category-theory.md) $(P,p_1,p_2)$ and $(Q,q_1,q_2)$ exist, the universal properties give unique arrows $f:P\to Q$ and $g:Q\to P$ respecting projections. The composites $gf$ and $fg$ respect the same projections as the identities, so uniqueness forces them to be identities. Thus a definition yields a genuine theorem: [products in a category](../../../../../product-category-theory.md) are unique up to unique compatible isomorphism. The proof matters because it licenses replacing a construction by any other realization of the same property.

The [Yoneda lemma](../../../../../yoneda-lemma.md) is a more substantial example. For a covariant [representable functor](../../../../../representable-functor.md) $\mathcal C(A,-)$ and $X:\mathcal C\to\mathbf{Set}$, a [natural transformation](../../../../../natural-transformation.md) $t:\mathcal C(A,-)\to X$ is determined by $a=t_A(1_A)$. [Naturality](../../../../../naturality.md) forces

$$
t_B(f)=X(f)(a).
$$

Conversely this formula defines a [natural transformation](../../../../../natural-transformation.md) for every $a\in X(A)$. Hence $\operatorname{Nat}(\mathcal C(A,-),X)\cong X(A)$. The definition of [naturality](../../../../../naturality.md) is indispensable, but the theorem identifies every possible transformation, proves representables detect arrows, and explains why universal objects can be studied through [hom-sets](../../../../../hom-set.md). Merely knowing the definition does not supply this conclusion.

Similarly, an [adjunction](../../../../../adjoint-functors.md) is defined by natural [hom-set](../../../../../hom-set.md) bijections. The construction of a [free abelian group](../../../../../free-abelian-group.md) gives $\mathbf{Ab}(\mathbb Z^{(S)},A)\cong\mathbf{Set}(S,UA)$, because a [group homomorphism](../../../../../group-homomorphism.md) is determined uniquely by its values on the basis. This makes a universal extension problem transparent. But the [Freyd general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md) goes further: it turns [categorical limit](../../../../../categorical-limit.md) preservation and a solution set into an actual adjoint. Its smallness hypotheses cannot be discarded as bookkeeping. For instance, the underlying-set [functor](../../../../../functor.md) from finite groups to finite sets has no left adjoint at a singleton. A putative universal finite [group](../../../../../group-split.md) with universal element of order $m$ could not map that element to a generator of a finite cyclic group of order greater than $m$. The theorem's hypotheses separate existence from attractive notation.

The [monoidal coherence theorem](../../../../../monoidal-coherence-theorem.md) offers another example. A [monoidal category](../../../../../monoidal-category.md) has associativity and unit isomorphisms satisfying the [pentagon identity for a monoidal category](../../../../../pentagon-identity-for-a-monoidal-category.md) and [triangle identity for a monoidal category](../../../../../triangle-identity-for-a-monoidal-category.md). Coherence proves that every formal reassociation and unit insertion produces the same structural map. This is what justifies calculating without displaying all parentheses; it is not true merely because one has named an [associator](../../../../../associator.md). Nor does it identify arbitrary additional maps, such as distinct braidings.

Finally, the [opposite category](../../../../../opposite-category.md) construction shows how a definition can economize on proofs: reversing arrows takes [products in a category](../../../../../product-category-theory.md) to [coproducts in a category](../../../../../coproduct.md), [initial objects](../../../../../initial-object.md) to [terminal objects](../../../../../terminal-object.md) and [monads](../../../../../monad.md) to comonads. Yet this economy works because theorems and their proofs are invariant under the reversal. The subject is powerful precisely when definitions isolate reusable structure and theorems establish its consequences. Separating their importance obscures that partnership.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
