<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A signature $\Sigma$ specifies sorts, finite-arity function symbols and finite-arity relation symbols. A [coherent formula](../../../../../coherent-formula.md) is built from atomic relations and equality using $\top,\bot$, finite conjunction, finite disjunction and existential quantification. A [coherent theory](../../../../../coherent-theory.md) consists of [coherent sequents](../../../../../coherent-sequent.md) $\phi\vdash_{\vec x}\psi$ in finite typed contexts. The context expresses universal quantification of the free variables; unrestricted universal quantification or negation is not a formula constructor here.

Construct the [coherent syntactic category](../../../../../coherent-syntactic-category.md) $\mathcal C_{\mathbb T}$ as follows. Objects are formulas in context $\{\vec x.\phi\}$, modulo renaming and provable equivalence. An arrow to $\{\vec y.\psi\}$ is a formula $\rho(\vec x,\vec y)$, modulo provable equivalence, for which the theory proves

$$
\rho\vdash\phi\wedge\psi,\qquad\phi\vdash_{\vec x}\exists\vec y\,\rho,\qquad\rho(\vec x,\vec y)\wedge\rho(\vec x,\vec y')\vdash\vec y=\vec y'.
$$

These say that the relation is supported on the specified objects, total and single-valued. The identity is equality on the context, and composition is

$$
(\sigma\circ\rho)(\vec x,\vec z)=\exists\vec y\,(\rho(\vec x,\vec y)\wedge\sigma(\vec y,\vec z)).
$$

The logical rules give associativity and the identity laws. The empty-context true formula is terminal; conjunction in disjoint contexts gives products; conjunction with equality of the two functional relations gives [equalizers](../../../../../equaliser.md). Existential quantification gives images, and finite disjunction gives unions of [subobjects](../../../../../subobject.md). Substitution preserves these constructions, so images and unions are stable under pullback. This makes $\mathcal C_{\mathbb T}$ a [coherent category](../../../../../coherent-category.md).

Let $M$ be a $\mathbb T$-model in a [topos](../../../../../elementary-topos.md) $\mathcal E$. Interpret each context as a finite product of its sort objects and each formula as its corresponding [subobject](../../../../../subobject.md). Define

$$
F_M(\{\vec x.\phi\})=\llbracket\vec x.\phi\rrbracket_M.
$$

The interpretation of an arrow relation $\rho$ is a total single-valued relation between these objects. Its projection to the domain is both an [epimorphism](../../../../../epimorphism.md), by totality, and a [monomorphism](../../../../../monomorphism.md), by single-valuedness, hence invertible in a topos. Its other projection therefore determines a unique morphism. Composition agrees with relational composition, so $F_M$ is a [functor](../../../../../functor.md). Finite limits interpret equality and conjunction; images interpret existential quantification; finite unions interpret disjunction, including the empty union for $\bot$. Consequently $F_M$ is a [coherent functor](../../../../../coherent-functor.md).

Conversely there is a canonical syntactic model $U$ in $\mathcal C_{\mathbb T}$. Interpret a sort $s$ by $\{x:s.\top\}$, a function symbol by its term graph, and a relation symbol by its atomic formula-in-context [subobject](../../../../../subobject.md). Induction on formulas identifies the interpretation of every $\phi$ in $U$ with its formula-in-context object. Every axiom is then an inclusion of the associated [subobjects](../../../../../subobject.md), because it is provable in $\mathbb T$.

For a [coherent functor](../../../../../coherent-functor.md) $F:\mathcal C_{\mathbb T}\to\mathcal E$, set $M_F=F(U)$. Preservation of [finite limits](../../../../../finite-limit.md), images and unions proves inductively that $F$ preserves all coherent interpretations, so every axiom holds in $M_F$. The same induction supplies natural isomorphisms

$$
F(\{\vec x.\phi\})\cong\llbracket\vec x.\phi\rrbracket_{M_F},
$$

compatible with the functional relations defining arrows. Thus $F\cong F_{M_F}$; directly on the sorts, operations and relations, $M_{F_M}\cong M$.

Finally these constructions agree on morphisms. A model homomorphism $h:M\to N$ induces maps on finite contexts. Atomic relations are preserved by definition; finite conjunction and disjunction and existential witnesses then show that each formula object maps to the corresponding formula object. Compatibility with functional relations makes these maps a [natural transformation](../../../../../natural-transformation.md) $F_M\to F_N$. Conversely a [natural transformation](../../../../../natural-transformation.md) between [coherent functors](../../../../../coherent-functor.md) restricts to its components on sort objects; naturality for term graphs preserves operations, and naturality for relation inclusions preserves relations. It is therefore a model homomorphism. The two correspondences are inverse. We have proved the categorical, not merely objectwise, equivalence

$$
\boxed{\operatorname{Mod}_{\mathbb T}(\mathcal E)\simeq\operatorname{Coh}(\mathcal C_{\mathbb T},\mathcal E).}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
