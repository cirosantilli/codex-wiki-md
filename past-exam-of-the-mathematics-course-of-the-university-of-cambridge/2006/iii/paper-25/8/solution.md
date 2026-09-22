<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For the [Ehrenfeucht-Mostowski theorem](../../../../../ehrenfeucht-mostowski-theorem.md), start with an infinite structure $M$ and a [total order](../../../../../total-order.md) $I$. Choose a [Skolem expansion](../../../../../skolem-expansion.md) $M^*$, and adjoin constants $c_i$ for $i\in I$. Require the [elementary diagram](../../../../../elementary-diagram-of-a-structure.md) of $M^*$, distinctness of these new constants, and the [order-indiscernible sequence](../../../../../order-indiscernible-sequence.md) schema: any two increasing tuples of the $c_i$ of the same length satisfy the same [first-order formulas](../../../../../first-order-formula.md) in the expanded language. Every finite fragment mentions finitely many new constants and finitely many [first-order formulas](../../../../../first-order-formula.md). Enumerate a countably infinite subset of $M$. For each of the finitely many [first-order formulas](../../../../../first-order-formula.md), color its increasing tuples by its truth value in $M^*$, including whatever fixed parameters occur in the fragment. Successive applications of the infinite [Ramsey theorem](../../../../../ramsey-theorem.md) leave an infinite [subset](../../../../../subset.md) homogeneous for all these colorings. Assign the finitely many new constants to distinct elements of this [subset](../../../../../subset.md) in their index order. Their finite indiscernibility requirements and the [elementary diagram](../../../../../elementary-diagram-of-a-structure.md) are then simultaneously satisfied.

The [compactness theorem](../../../../../compactness-theorem.md) supplies an [elementary extension](../../../../../elementary-extension.md) $N^*$ containing the required distinct indiscernibles. Their [Skolem hull](../../../../../skolem-hull.md) is an [elementary substructure](../../../../../elementary-substructure.md): an existential [first-order formula](../../../../../first-order-formula.md) true of its elements has its chosen Skolem-function witness in the hull, so the [Tarski-Vaught test](../../../../../tarski-vaught-test.md) applies. Any [order automorphism](../../../../../order-automorphism.md) $\sigma$ of $I$ acts on this hull by

$$
t(c_{i_1},\ldots,c_{i_n})\longmapsto t(c_{\sigma(i_1)},\ldots,c_{\sigma(i_n)}).
$$

Indiscernibility makes this well defined, since every equality of two term representations is preserved. The same argument preserves every [first-order formula](../../../../../first-order-formula.md); the inverse is given by $\sigma^{-1}$. Thus it is an automorphism, uniquely determined in the language of the chosen [Skolem expansion](../../../../../skolem-expansion.md) by its values on the generators. This proves both the indiscernible-model and automorphism forms of the [Ehrenfeucht-Mostowski theorem](../../../../../ehrenfeucht-mostowski-theorem.md). Uniqueness is not claimed for automorphisms of the reduct which need not preserve the chosen [Skolem functions](../../../../../skolem-function.md).

For [simple typed set theory with atoms](../../../../../simple-typed-set-theory-with-atoms.md), write $S_i$ for the [set](../../../../../set-split.md) predicate at sort $i$. Members have sort one lower; [urelements](../../../../../urelement.md) have no typed members, [extensionality](../../../../../axiom-of-extensionality.md) applies to [sets](../../../../../set-split.md), and every well-typed [first-order formula](../../../../../first-order-formula.md) defines a [set](../../../../../set-split.md) at the next sort. [Typical ambiguity](../../../../../typical-ambiguity.md) adds $\phi\leftrightarrow\phi^+$ for each closed sentence, where $+$ raises every sort by one. We prove finite satisfiability using [Ramsey theorem](../../../../../ramsey-theorem.md), rather than assuming that adjacent sorts have the same [cardinality](../../../../../cardinality.md).

Let $X_n=V_{\omega+2n}$. If $n<m$, then $\mathcal P(X_n)\subseteq X_m$. For increasing integers $h_0<h_1<h_2<\cdots$, interpret sort $i$ by $D_i=X_{h_{i+1}}$, interpret $S_i$ by the objects of $\mathcal P(X_{h_i})$, and interpret adjacent-sort membership by actual membership restricted to these designated [sets](../../../../../set-split.md). All other objects of a sort are typed [urelements](../../../../../urelement.md). Every [subset](../../../../../subset.md) of $D_i$ is a designated [set](../../../../../set-split.md) in $D_{i+1}$, so comprehension holds for every [first-order formula](../../../../../first-order-formula.md), including [first-order formulas](../../../../../first-order-formula.md) with quantifiers and parameters at other sorts. Two designated [sets](../../../../../set-split.md) with the same members are equal, while the other objects have no typed members. Thus this is a full model of the typed axioms for every increasing [sequence](../../../../../sequence.md) of levels. The extra preceding level $h_0$ gives a consistent interpretation of the bottom [set](../../../../../set-split.md) predicate as well.

Take finitely many ambiguity sentences and let $r$ bound their highest sort before raising. Color increasing $(r+2)$-tuples $(h_0,\ldots,h_{r+1})$ by the vector of truth values of these sentences in the corresponding finite sorted structure. There are finitely many colors. The infinite [Ramsey theorem](../../../../../ramsey-theorem.md) supplies an [homogeneous set](../../../../../homogeneous-set-for-a-colouring.md) of indices. Choose the level [sequence](../../../../../sequence.md) from it. The sentence $\phi$ is evaluated in the window $(h_0,\ldots,h_{r+1})$, while $\phi^+$ is evaluated in the next window $(h_1,\ldots,h_{r+2})$; homogeneity makes their truth values equal. Sentences using fewer sorts simply ignore the unused final levels. Thus every finite family of ambiguity axioms has a model satisfying all the typed axioms. Apply many-sorted first-order [compactness theorem](../../../../../compactness-theorem.md) to obtain

$$
\boxed{\operatorname{Con}(\mathrm{TSTU}+\mathrm{Typical\ Ambiguity}).}
$$

This is a relative consistency construction in the ordinary set-theoretic metatheory. Allowing urelements is essential here: skipping ranks leaves objects outside the represented [power sets](../../../../../power-set.md), and those objects must be permitted as [urelements](../../../../../urelement.md).

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
