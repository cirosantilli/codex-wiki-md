<h1 id="7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

One useful form of the [Ehrenfeucht-Mostowski theorem](../../../../../../ehrenfeucht-mostowski-theorem.md) is this: for an infinite [first-order structure](../../../../../../first-order-structure.md) $A$ and any total order $I$, there is a [first-order model](../../../../../../model-of-a-first-order-theory.md) of $\operatorname{Th}(A)$ generated in a chosen [Skolem expansion](../../../../../../skolem-expansion.md) by an [order-indiscernible sequence](../../../../../../order-indiscernible-sequence.md) $(c_i)_{i\in I}$ of distinct elements. Every [order automorphism](../../../../../../order-automorphism.md) of $I$ induces an [structure automorphism](../../../../../../automorphism-of-a-first-order-structure.md) of this expanded hull. One can additionally obtain an [elementary extension](../../../../../../elementary-extension.md) containing $A$ by including its [elementary diagram](../../../../../../elementary-diagram-of-a-structure.md). Uniqueness of the induced [structure automorphism](../../../../../../automorphism-of-a-first-order-structure.md) is asserted in the [Skolem expansion](../../../../../../skolem-expansion.md), not among arbitrary [structure automorphisms](../../../../../../automorphism-of-a-first-order-structure.md) of the reduct.

Choose a [Skolem expansion](../../../../../../skolem-expansion.md) $A^*$: for every existential [first-order formula](../../../../../../first-order-formula.md) choose a witness [function](../../../../../../function-split.md), satisfying $\exists y\,\varphi(y,\bar x)\Rightarrow\varphi(f_\varphi(\bar x),\bar x)$. Iterate the expansion if necessary so witnesses are available for [first-order formulas](../../../../../../first-order-formula.md) in the resulting language. Add constants $c_i$ and require $c_i\ne c_j$ for distinct indices. For every [first-order formula](../../../../../../first-order-formula.md) $\varphi(x_1,\ldots,x_m)$ of the expanded language and every two increasing index tuples, add

$$
\varphi(c_{i_1},\ldots,c_{i_m})\longleftrightarrow
\varphi(c_{j_1},\ldots,c_{j_m}).
$$

Together with $\operatorname{Th}(A^*)$, this is the indiscernibility theory.

Every finite fragment is satisfiable. It mentions only finitely many [first-order formulas](../../../../../../first-order-formula.md) and index constants. Choose a countably infinite [sequence](../../../../../../sequence.md) of distinct elements of $A^*$. For each relevant arity, colour increasing tuples from that [sequence](../../../../../../sequence.md) by the finite truth vector of all [first-order formulas](../../../../../../first-order-formula.md) of that arity in the fragment. Successive applications of the infinite [Ramsey theorem for r-sets](../../../../../../ramsey-s-theorem.md) leave an infinite [subset](../../../../../../subset.md) homogeneous for each of these finitely many finite colourings. Interpret the finitely many index constants by distinct elements of that [subset](../../../../../../subset.md) in increasing enumeration order. All the required truth-value equivalences then hold, and the original structure satisfies the finite part of its own theory.

If an actual [elementary extension](../../../../../../elementary-extension.md) of $A$ is desired, include constants for its elements and the [elementary diagram](../../../../../../elementary-diagram-of-a-structure.md) of $A^*$. A finite fragment still contains only finitely many parameter instances; include those truth vectors in the same colourings. Thus finite satisfiability is unchanged. The [compactness theorem](../../../../../../compactness-theorem.md) now supplies a [first-order model](../../../../../../model-of-a-first-order-theory.md) with the entire indiscernible [sequence](../../../../../../sequence.md), and in the diagram version an elementary copy of $A$.

Take the [Skolem hull](../../../../../../skolem-hull.md) of the generators, including the diagram constants when present. The witness [functions](../../../../../../function-split.md) show directly that the hull is elementary: whenever an existential [first-order formula](../../../../../../first-order-formula.md) with hull parameters is true in the ambient [first-order model](../../../../../../model-of-a-first-order-theory.md), its Skolem witness belongs to the hull. Induction on [first-order formulas](../../../../../../first-order-formula.md), or the [Tarski-Vaught test](../../../../../../tarski-vaught-test.md), gives elementarity. Its reduct is therefore a [first-order model](../../../../../../model-of-a-first-order-theory.md) of $\operatorname{Th}(A)$. In the version without diagram constants its [cardinality](../../../../../../cardinality.md) is at most $\max(|I|,|\mathcal L|,\aleph_0)$.

For an [order automorphism](../../../../../../order-automorphism.md) $\rho:I\to I$, define

$$
\widehat\rho\bigl(t(c_{i_1},\ldots,c_{i_m})\bigr)
=t(c_{\rho(i_1)},\ldots,c_{\rho(i_m)}).
$$

This is well defined. If two terms represent the same element, express their equality as a [first-order formula](../../../../../../first-order-formula.md) on the increasing [union](../../../../../../set-union.md) of their generator indices. Indiscernibility and preservation of the index order carry that equality to the transported terms. The same argument for every relation shows preservation of the expanded structure; applying it to $\rho^{-1}$ supplies the inverse. Every element is a term in the generators, so no other [structure automorphism](../../../../../../automorphism-of-a-first-order-structure.md) of the specified expansion can have the same action on them. Hence

$$
\boxed{\text{order automorphisms of }I\text{ extend uniquely to the generated Skolem expansion.}}
$$

For an application requiring the generators to lie in a definable infinite ordered class, impose that class predicate and its increasing-order [first-order formulas](../../../../../../first-order-formula.md) too. The finite-fragment proof uses an increasing [sequence](../../../../../../sequence.md) in that class, so all these additional conditions are preserved. In particular the integer index order and its shift give the [structure automorphism](../../../../../../automorphism-of-a-first-order-structure.md) used in the [NFU](../../../../../../new-foundations-with-urelements.md) construction. The constants are order indiscernibles, not necessarily indiscernibles under arbitrary permutations of the index [set](../../../../../../set-split.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7](../../7.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
