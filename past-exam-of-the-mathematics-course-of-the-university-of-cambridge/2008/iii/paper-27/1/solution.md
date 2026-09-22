<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Ehrenfeucht-Mostowski theorem](../../../../../ehrenfeucht-mostowski-theorem.md) says that an infinite [first-order structure](../../../../../first-order-structure.md) $M$, after [Skolem expansion](../../../../../skolem-expansion.md), has an elementarily equivalent model generated as a [Skolem hull](../../../../../skolem-hull.md) by distinct [order-indiscernible sequence](../../../../../order-indiscernible-sequence.md) $(a_i)_{i\in I}$ for any prescribed linear order $I$. Every [order automorphism](../../../../../order-automorphism.md) of $I$ extends uniquely to an automorphism preserving this [Skolem expansion](../../../../../skolem-expansion.md). The reduct still models $\operatorname{Th}(M)$, but uniqueness of an automorphism in the reduct alone is not asserted. Iterate adjoining witness functions through all successively enlarged languages, so every existential formula in the final language has its own [Skolem function](../../../../../skolem-function.md). Write $M^*$ for the resulting expanded structure.

For the [Ramsey theorem](../../../../../ramsey-theorem.md) proof, add constants $c_i$ and require that they are distinct and that every two increasing tuples of the same length agree on every formula of the expanded language. Include $\operatorname{Th}(M^*)$. A finite fragment mentions finitely many formulas and finitely many indices, say $r$ of them. Choose distinct $b_n\in M$. For each arity occurring in those formulas, color the increasing tuples of [natural numbers](../../../../../natural-number.md) by their finite truth vectors in $M^*$. Repeated applications of the infinite [Ramsey theorem](../../../../../ramsey-theorem.md) give an infinite subset homogeneous for all these finitely many colorings. Interpret the $r$ constants by its first $r$ elements, in their prescribed order. All the fragment's indiscernibility requirements hold. Thus [compactness theorem](../../../../../compactness-theorem.md) produces a model $N^*$ of the whole scheme.

Let $H$ be the [Skolem hull](../../../../../skolem-hull.md) of the $c_i$. Whenever an existential formula with parameters in $H$ holds in $N^*$, its chosen Skolem witness belongs to $H$. The [Tarski-Vaught test](../../../../../tarski-vaught-test.md), proved by the existential step of induction on formulas, therefore makes $H\prec N^*$. For an [order automorphism](../../../../../order-automorphism.md) $\rho:I\to I$, define

$$
\widehat\rho\bigl(t(c_{i_1},\ldots,c_{i_r})\bigr)
=t(c_{\rho(i_1)},\ldots,c_{\rho(i_r)}).
$$

To compare different term presentations, collect all their indices into one increasing tuple. Indiscernibility transfers the equality of the terms to the transported tuple, so this map is well defined. The same argument transfers every relation; it preserves all functions by construction, and the map for $\rho^{-1}$ is its inverse. Since every hull element is a term in the generators, uniqueness follows.

For a genuinely [ultraproduct](../../../../../ultraproduct.md) proof, keep the distinct $b_n$ and choose a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) $\mathcal U$ on $\mathbb N$. For each finite ordered subset $F\subset I$, take

$$
M_F=(M^*)^{\mathbb N^F}/\mathcal U_F,
$$

where $\mathcal U_F$ is the ordered [Fubini product of ultrafilters](../../../../../fubini-product-of-ultrafilters.md). Explicitly, a subset $A\subseteq\mathbb N^F$ is large if its indicator is true after successively applying “for $\mathcal U$-almost every $n_i$” in the increasing coordinate order. Projection to any sublist has exactly that sublist's product [ultrafilter](../../../../../ultrafilter.md). Hence for $F\subseteq G$, pulling functions back along $\mathbb N^G\to\mathbb N^F$ gives an [elementary embedding](../../../../../elementary-embedding.md) $M_F\to M_G$ by the [Łoś theorem](../../../../../los-theorem.md). These embeddings commute. Form their [directed limit of elementary embeddings](../../../../../directed-limit-of-elementary-embeddings.md); each finite tuple lies in one stage, so induction on formulas makes the stage embeddings elementary.

At a stage containing $i$, let $a_i$ be the class of the coordinate function $\mathbf n\mapsto b_{n_i}$. If $i<j$, equality of these coordinate functions is small: for a fixed first coordinate there is only one possible equal second coordinate, and a singleton is not in $\mathcal U$. Thus $a_i\ne a_j$. For any increasing $i_1<\cdots<i_r$, the truth of $\varphi(a_{i_1},\ldots,a_{i_r})$ is the same nested [ultrafilter](../../../../../ultrafilter.md) test applied to $\varphi(b_{n_1},\ldots,b_{n_r})$, independent of the actual indices. This is precisely indiscernibility in the expanded language. Its [Skolem hull](../../../../../skolem-hull.md), and the term-transport construction above, finish the second proof. **Both constructions give the required model and the extended index automorphisms.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
