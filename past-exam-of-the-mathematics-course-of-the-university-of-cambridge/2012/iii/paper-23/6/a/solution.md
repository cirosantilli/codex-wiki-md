<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [geometric formula](../../../../../../geometric-formula.md) is built from atomic formulas, including equality, using finite conjunctions, arbitrary set-indexed disjunctions and existential quantification in a finite variable context. Truth is the empty conjunction and falsity the empty disjunction. A [geometric theory](../../../../../../geometric-theory.md) is a set of sequents $\phi\vdash_{\vec x}\psi$ between such formulas over a many-sorted signature. The context supplies the universal force of an axiom; unrestricted universal quantification, implication and negation are not formula constructors in this fragment.

These choices are exactly suited to [inverse image functors of geometric morphisms](../../../../../../inverse-image-functor-of-a-geometric-morphism.md). Finite-limit preservation handles equality and conjunction; [colimit](../../../../../../colimit.md) and image preservation handle disjunction and existential quantification. Therefore an inverse image carries an internal model of a [geometric theory](../../../../../../geometric-theory.md) to another model.

Construct the [geometric syntactic category](../../../../../../geometric-syntactic-category.md) $\mathcal C_{\mathbb T}$ as follows. Objects are formulas in context $\{\vec x.\phi\}$, modulo provable renaming and equivalence. A morphism to $\{\vec y.\psi\}$ is an equivalence class of formulas $\theta(\vec x,\vec y)$ that are provably total and single-valued:

$$
\theta\vdash\phi\wedge\psi,\qquad
\phi\vdash_{\vec x}\exists\vec y\,\theta,\qquad
\theta(\vec x,\vec y)\wedge\theta(\vec x,\vec y')
\vdash_{\vec x,\vec y,\vec y'}\vec y=\vec y'.
$$

The last notation abbreviates componentwise equality. Identity is equality of the context variables; composition is existential conjunction over the intermediate tuple. The category has [finite limits](../../../../../../finite-limit.md), formed through conjunction and equality.

Give it the [geometric syntactic topology](../../../../../../geometric-syntactic-topology.md) $J_{\mathbb T}$. A family of arrows represented by $\theta_i(\vec y_i,\vec x)$ into $\{\vec x.\phi\}$ covers when

$$
\mathbb T\vdash_{\vec x}
\phi\ \Longrightarrow\ \bigvee_i\exists\vec y_i\,\theta_i(\vec y_i,\vec x).
$$

Pullback stability is substitution, and transitivity comes from distributing existential conjunction through the covering disjunctions. Thus the generated sieves define a [Grothendieck topology](../../../../../../grothendieck-topology.md). Empty covers impose the interpretation of falsity as the [initial object](../../../../../../initial-object.md).

The [classifying topos](../../../../../../classifying-topos.md) is

$$
\boxed{\mathbf{Set}[\mathbb T]=
\mathbf{Sh}(\mathcal C_{\mathbb T},J_{\mathbb T}).}
$$

Its universal model $U_{\mathbb T}$ assigns a sort $A$ the sheafified representable of $\{x^A.\top\}$, functions their definable graph morphisms and relations their definable [subobjects](../../../../../../subobject.md). The syntactic covering conditions make the axioms valid in this model.

For the universal property, interpreting formulas in a model $M$ in a [Grothendieck topos](../../../../../../grothendieck-topos.md) $\mathcal F$ gives a finite-limit-preserving, $J_{\mathbb T}$-continuous [functor](../../../../../../functor.md) $\mathcal C_{\mathbb T}\to\mathcal F$: covers go to jointly epimorphic families precisely because the relevant sequents hold. The [Diaconescu equivalence for geometric morphisms](../../../../../../diaconescu-equivalence-for-geometric-morphisms.md) associates to this [functor](../../../../../../functor.md) a [geometric morphism](../../../../../../geometric-morphism.md) $\mathcal F\to\mathbf{Set}[\mathbb T]$. Conversely, pulling $U_{\mathbb T}$ back along a [geometric morphism](../../../../../../geometric-morphism.md) gives a model. The constructions on models and their homomorphisms are inverse up to [natural isomorphism](../../../../../../natural-isomorphism.md), yielding

$$
\boxed{\operatorname{Geom}(\mathcal F,\mathbf{Set}[\mathbb T])
\simeq\mathbb T\operatorname{-Mod}(\mathcal F)}
$$

naturally in $\mathcal F$. This proves the required classifying property, not merely classification of set-valued models.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
