<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A useful form of the [Ehrenfeucht-Mostowski theorem](../../../../../../ehrenfeucht-mostowski-theorem.md) says that, for an infinite [first-order structure](../../../../../../first-order-structure.md) $M$ and any total order $I$, there is a model of $\operatorname{Th}(M)$ generated as a [Skolem hull](../../../../../../skolem-hull.md) by distinct order indiscernibles $(a_i)_{i\in I}$. Every [order automorphism](../../../../../../order-automorphism.md) of $I$ extends uniquely to an [automorphism](../../../../../../automorphism.md) of the specified [Skolem expansion](../../../../../../skolem-expansion.md) of that hull. The model can be obtained inside an [elementary extension](../../../../../../elementary-extension.md) of a [Skolem expansion](../../../../../../skolem-expansion.md) of $M$; the generated hull itself need not contain $M$.

Choose a [Skolem expansion](../../../../../../skolem-expansion.md) $M^*$ by iteratively adjoining witness functions: for each existential formula in the current language choose a function returning a witness whenever one exists, with an arbitrary value otherwise. Repeat for countably many rounds. Every formula in the final language uses finitely many symbols, so has a witness function from a later round. Thus the expansion is Skolemized for its own formulas, as required for elementarity of its hull. Add constants $a_i$ for $i\in I$ to the complete theory of $M^*$, require them to be distinct, and impose the scheme

$$
\varphi(a_{i_1},\ldots,a_{i_n})\longleftrightarrow\varphi(a_{j_1},\ldots,a_{j_n})
\quad(i_1<\cdots<i_n,\ j_1<\cdots<j_n)
$$

for every formula in the Skolem language. If an [elementary extension](../../../../../../elementary-extension.md) of $M^*$ is desired, also add its [elementary diagram](../../../../../../elementary-diagram-of-a-structure.md) with separate names for its elements.

Every finite part of this theory is satisfiable. Choose infinitely many distinct elements $b_0,b_1,\ldots$ of $M$. For each of the finitely many arities in that fragment, color increasing index tuples by the finite vector of truth values of the formulas occurring. Repeated applications of the infinite Ramsey theorem give an infinite [subset](../../../../../../subset.md) on which all these vectors are constant. Interpret the finitely many $a_i$ in increasing-index order from that [subset](../../../../../../subset.md). This satisfies the finite indiscernibility requirements and distinctness, while the [elementary diagram](../../../../../../elementary-diagram-of-a-structure.md) is satisfied by the named original structure. The [compactness theorem](../../../../../../compactness-theorem.md) gives a structure $N^*$ satisfying the whole theory.

Let $H$ be the closure of the $a_i$ under the [Skolem functions](../../../../../../skolem-function.md), including nullary ones. It is elementary in $N^*$: whenever an existential formula with parameters from $H$ is true in $N^*$, its Skolem witness lies in $H$. This is the [Tarski-Vaught test](../../../../../../tarski-vaught-test.md), whose proof is [induction](../../../../../../mathematical-induction.md) on formulas, using precisely this witness property for the existential step. Hence the reduct of $H$ is a model of $\operatorname{Th}(M)$.

For an [order automorphism](../../../../../../order-automorphism.md) $\sigma:I\to I$, define

$$
\widehat\sigma\bigl(t(a_{i_1},\ldots,a_{i_n})\bigr)=t(a_{\sigma(i_1)},\ldots,a_{\sigma(i_n)}).
$$

This is well-defined. If two terms denote the same element, write their equality as a formula on the combined increasing tuple of their indices; indiscernibility preserves that formula after transport by $\sigma$. The same argument preserves every relation and function. Applying $\sigma^{-1}$ gives the inverse, so $\widehat\sigma$ is an [automorphism](../../../../../../automorphism.md). Since all elements are terms in the generators, it is the unique [automorphism](../../../../../../automorphism.md) of this [Skolem expansion](../../../../../../skolem-expansion.md) extending $a_i\mapsto a_{\sigma(i)}$. This proves the theorem.

One may require the indiscernibles to lie in any specified infinite [sequence](../../../../../../sequence.md) of the starting structure, or to satisfy additional finite-tuple properties holding along that [sequence](../../../../../../sequence.md): the same finite satisfiability proof chooses its homogeneous [subsequence](../../../../../../subsequence.md) there. This strengthened form is what the rank-domain construction of [NFU](../../../../../../new-foundations-with-urelements.md) uses. **Uniqueness is asserted in the [Skolem expansion](../../../../../../skolem-expansion.md), not for all [automorphisms](../../../../../../automorphism.md) of its reduct.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
