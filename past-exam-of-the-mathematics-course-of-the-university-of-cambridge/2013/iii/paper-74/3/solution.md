<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Cartesian theory](../../../../../cartesian-theory.md) has a many-sorted [first-order signature](../../../../../first-order-signature.md), with finite arities, and axioms expressed as sequents between [Cartesian formulas](../../../../../cartesian-formula.md). Those formulas use atomic relations and equality, truth and finite [logical conjunctions](../../../../../logical-conjunction.md). They also admit [existential quantification](../../../../../existential-quantification.md) when the quantified witness is provably unique: to form $\exists y\,\phi(x,y)$, require $\phi(x,y)\wedge\phi(x,y')\vdash y=y'$ relative to the theory. One can quantify a finite tuple in the same way. Arbitrary existential quantifiers, disjunction, negation and universal quantifiers are not formula constructors in this fragment. In particular falsity is not included as an additional finite-limit constructor. The universal force of a sequent comes from its free-variable context. This is the fragment whose categorical semantics requires exactly [finite limits](../../../../../finite-limit.md).

The [Cartesian syntactic category](../../../../../cartesian-syntactic-category.md) $\mathcal C_{\mathbb T}$ has objects $\{\vec x\mid\phi\}$, identifying harmless renamings and provably equivalent formulas-in-context. An arrow from $\{\vec x\mid\phi\}$ to $\{\vec y\mid\psi\}$ is represented by a provably functional Cartesian relation $\theta(\vec x,\vec y)$: it entails $\phi\wedge\psi$, is total on $\phi$, and has a unique output tuple. Provable equivalence identifies arrows. Equality supplies identity arrows; composition quantifies the uniquely determined intermediate tuple in a conjunction. Totality and uniqueness prove that the composite is again functional.

The empty truth context is terminal. Products concatenate disjoint contexts and conjoin their formulas. A [pullback](../../../../../pullback-category-theory.md) of two functional relations adds the condition that their outputs agree; the common output is unique, so the existential quantification used to express it is Cartesian. This gives all [finite limits](../../../../../finite-limit.md) and makes the usual equality diagrams into [equalizers](../../../../../equaliser.md).

An internal model $M$ in a finite-limit category $\mathcal E$ interprets each sort by an object, functions by arrows and relations by [subobjects](../../../../../subobject.md). Equality is a diagonal and conjunction is a [pullback](../../../../../pullback-category-theory.md) intersection. A uniquely witnessed relation projects monomorphically onto the context, so its existential interpretation needs no general image operation: it is that mono. Evaluating formulas and functional relations yields a [finite-limit-preserving functor](../../../../../finite-limit-preserving-functor.md) $F_M:\mathcal C_{\mathbb T}\to\mathcal E$.

Conversely, the canonical syntactic model uses the single-sort truth contexts, term graphs and atomic [subobjects](../../../../../subobject.md). Its interpretation of a formula is the formula-in-context object itself. Applying any [finite-limit-preserving functor](../../../../../finite-limit-preserving-functor.md) supplies a model and preserves its axioms. These constructions are inverse up to the natural interpretation isomorphisms; model homomorphisms correspond to [natural transformations](../../../../../natural-transformation.md). Therefore

$$
\boxed{\operatorname{Lex}(\mathcal C_{\mathbb T},\mathcal E)\simeq\mathbb T\text{-}\operatorname{Mod}(\mathcal E).}
$$

For completeness, let a sequent in context be represented by [subobjects](../../../../../subobject.md) $i:A\hookrightarrow C$ and $j:B\hookrightarrow C$ for its antecedent and consequent. Derivability is exactly the existence of a factorization $i=jv$ in the syntactic category. Consider the covariant [representable functor](../../../../../representable-functor.md) $\mathcal C_{\mathbb T}(A,-)$, which preserves all existing limits, and hence corresponds to a set-valued model. In that model the element $i\in\mathcal C_{\mathbb T}(A,C)$ belongs to the antecedent, because it is the image of $1_A$. If the sequent holds, it also belongs to the consequent, so $i=jv$ for some $v:A\to B$. That is precisely a derivation of the sequent. Thus **validity in all set-valued models implies Cartesian derivability**. More concretely, every underivable sequent is refuted by this representable model. No assumption that every sort is inhabited is needed: some hom-sets may be empty.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
