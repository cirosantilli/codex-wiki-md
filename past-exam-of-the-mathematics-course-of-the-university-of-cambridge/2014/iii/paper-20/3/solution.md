<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [first-order signature](../../../../../first-order-signature.md) specifies sorts, function symbols with specified input and output sorts, and relation symbols with specified input sorts. A [coherent formula](../../../../../coherent-formula.md) is built from atomic relations and equalities using $\top$, $\bot$, finite [logical conjunctions](../../../../../logical-conjunction.md), finite [logical disjunctions](../../../../../logical-disjunction.md), and [existential quantification](../../../../../existential-quantification.md). A [coherent theory](../../../../../coherent-theory.md) is a set of sequents $\phi\vdash_{\vec x}\psi$ between [coherent formulas](../../../../../coherent-formula.md) in a common finite context; its axioms are interpreted as universally closed implications. Neither general negation nor universal quantification is allowed inside [coherent formulas](../../../../../coherent-formula.md).

One complete presentation of [coherent logic](../../../../../coherent-logic.md) consists of the following axiom and rule schemes, together with the theory's sequents. All displayed formulas have compatible sorts and contexts, and bound variables can be renamed.

Identity and cut give $\phi\vdash\phi$ and

$$
\frac{\phi\vdash\psi\quad\psi\vdash\theta}{\phi\vdash\theta}.
$$

Substitution replaces the free variables of any derivable sequent by well-typed terms, avoiding capture. Contexts can be enlarged by unused variables, and permuted or renamed.

The finite-meet rules are $\phi\vdash\top$, $\phi\wedge\psi\vdash\phi$, $\phi\wedge\psi\vdash\psi$, and

$$
\frac{\theta\vdash\phi\quad\theta\vdash\psi}{\theta\vdash\phi\wedge\psi}.
$$

The finite-join rules are $\bot\vdash\phi$, $\phi\vdash\phi\vee\psi$, $\psi\vdash\phi\vee\psi$, and

$$
\frac{\phi\vdash\theta\quad\psi\vdash\theta}{\phi\vee\psi\vdash\theta}.
$$

Include distributivity $\theta\wedge(\phi\vee\psi)\dashv\vdash(\theta\wedge\phi)\vee(\theta\wedge\psi)$.

Existential introduction is $\phi(\vec x,t)\vdash_{\vec x}\exists y\,\phi(\vec x,y)$. Existential elimination is

$$
\frac{\phi(\vec x,y)\vdash_{\vec x,y}\psi(\vec x)}{\exists y\,\phi(\vec x,y)\vdash_{\vec x}\psi(\vec x)},
$$

where $y$ is absent from $\psi$. Equivalently, the quantifier is [left adjoint](../../../../../adjoint-functors.md) to weakening along the context projection. Include the [Frobenius rule in coherent logic](../../../../../frobenius-rule-in-coherent-logic.md)

$$
\theta(\vec x)\wedge\exists y\,\phi(\vec x,y)\dashv\vdash\exists y\,(\theta(\vec x)\wedge\phi(\vec x,y)).
$$

It can also be derived from the usual coherent natural-deduction rules.

Equality has $\top\vdash_x x=x$ and the substitution scheme

$$
x=y\wedge\phi(\vec z,x)\vdash_{\vec z,x,y}\phi(\vec z,y),
$$

including atomic formulas and terms of the signature. Symmetry, transitivity and congruence for all functions and relations follow. These schemes impose no unintended inhabitedness axiom on a sort.

The [coherent syntactic category](../../../../../coherent-syntactic-category.md) $\mathcal C_{\mathbb T}$ has objects formulas in context $[\vec x\mid\phi]$, up to renaming. An arrow from $[\vec x\mid\phi]$ to $[\vec y\mid\psi]$ is an equivalence class, modulo provable equivalence, of formulas $\theta(\vec x,\vec y)$ satisfying

$$
\theta\vdash\phi\wedge\psi,\qquad\phi\vdash_{\vec x}\exists\vec y\,\theta,
$$

and

$$
\theta(\vec x,\vec y)\wedge\theta(\vec x,\vec y')\vdash\bigwedge_i y_i=y_i'.
$$

These are provably total functional relations. The identity is the equality graph restricted by $\phi$. If $\theta$ and $\rho$ are consecutive arrows, their composite is represented by $\exists\vec y\,(\theta\wedge\rho)$. Equality, cut and existential rules give the category laws.

A [coherent category](../../../../../coherent-category.md) has [finite limits](../../../../../finite-limit.md), [pullback](../../../../../pullback-category-theory.md)-stable regular-epi/mono image factorizations, and finite unions of [subobjects](../../../../../subobject.md) stable under [pullback](../../../../../pullback-category-theory.md). We verify these structures syntactically. The [terminal object](../../../../../terminal-object.md) is the empty-context truth formula. Products conjoin formulas in disjoint contexts; [equalizers](../../../../../equaliser.md) add equality of the two output tuples. For a functional relation $\theta$, its image in the target is represented by $\exists\vec x\,\theta$. Its factor onto that image is regular epic: two arrows out of the image agreeing on the source agree by existential elimination, and the same argument with the [kernel pair](../../../../../kernel-pair.md) gives the coequalizer property. Frobenius makes these image factorizations stable under [pullback](../../../../../pullback-category-theory.md).

Every [subobject](../../../../../subobject.md) of $[\vec x\mid\phi]$ is represented by a formula $\eta(\vec x)$ with $\eta\vdash\phi$. Indeed, take the existential image of a monic functional relation; uniqueness makes its map to that image an isomorphism. [Subobject](../../../../../subobject.md) inclusion is exactly provable implication. Finite unions are consequently disjunctions, with bottom as the empty [subobject](../../../../../subobject.md); distributivity and substitution make them [pullback](../../../../../pullback-category-theory.md)-stable. Hence **$\mathcal C_{\mathbb T}$ is coherent**.

The [conservative syntactic model](../../../../../conservative-syntactic-model.md) interprets a sort $S$ by $[x:S\mid\top]$, a function by its term graph, and a relation by its atomic-formula [subobject](../../../../../subobject.md). Induction on [coherent formulas](../../../../../coherent-formula.md) shows that $\phi(\vec x)$ is interpreted by the [subobject](../../../../../subobject.md) $[\vec x\mid\phi]$ of its context object. It satisfies every theory axiom by construction. Conversely, a sequent holds in this model exactly when the corresponding [subobject](../../../../../subobject.md) inclusion holds, which is exactly derivability in $\mathbb T$. Therefore

$$
\boxed{\text{the canonical model in }\mathcal C_{\mathbb T}\text{ is conservative}.}
$$

This is conservativity for [coherent sequents](../../../../../coherent-sequent.md), not a claim about non-[coherent formulas](../../../../../coherent-formula.md).

## ↑ Ancestors (11)

1. [3](../3.md)
2. [Section A](../section-a.md)
3. [Paper 20](../../paper-20-split.md)
4. [Iii](../../split.md)
5. [2014](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
