<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

One form of the [Ehrenfeucht-Mostowski theorem](../../../../../ehrenfeucht-mostowski-theorem.md) says that, for every infinite [first-order structure](../../../../../first-order-structure.md) $M$ and every [total order](../../../../../total-order.md) $I$, an [elementary extension](../../../../../elementary-extension.md) contains distinct elements $(a_i)_{i\in I}$ forming an [order-indiscernible sequence](../../../../../order-indiscernible-sequence.md). After a suitable [Skolem expansion](../../../../../skolem-expansion.md), their [Skolem hull](../../../../../skolem-hull.md) is a [first-order model](../../../../../model-of-a-first-order-theory.md) of $\operatorname{Th}(M)$, and every [order automorphism](../../../../../order-automorphism.md) of $I$ extends to a [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md) of that hull. If $M$ has a definable infinite linearly ordered subset $P$, the generators may lie in $P$ and their order may agree with that definable order. Uniqueness of the extended [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md) is asserted in the chosen [Skolem expansion](../../../../../skolem-expansion.md), rather than for every [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md) of its reduct.

Here is an [ultraproduct proof of the Ehrenfeucht-Mostowski theorem](../../../../../ultraproduct-proof-of-the-ehrenfeucht-mostowski-theorem.md). First expand $M$ to $M^+$ with [Skolem functions](../../../../../skolem-function.md) for all existential [first-order formulas](../../../../../first-order-formula.md), iterating through the enlarged languages if necessary. This is done in the ordinary classical metatheory; the choice restriction in question 1 is not a restriction on this question. Fix a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) $\mathcal U$ on $\mathbb N$.

We can obtain an infinite [sequence](../../../../../sequence.md) of distinct elements $b_0,b_1,\ldots$ in an [elementary extension](../../../../../elementary-extension.md) $M_0$ of $M^+$ by one preliminary [ultrapower](../../../../../ultrapower.md). For each $n\geq1$ choose a finite list of $n$ distinct elements of $M^+$. Represent $b_j$ by the [function](../../../../../function-split.md) taking the $j$th entry when $n>j$, with an arbitrary default otherwise. Distinctness holds on a [cofinite set](../../../../../cofinite-set.md), so follows from [Łoś theorem](../../../../../los-theorem.md). In the definably ordered variant, first name any parameters defining $P$, and choose each finite list increasingly inside $P$ instead; then $M_0\models P(b_j)$ and $b_j<b_k$ for $j<k$. Infinitude of an ordered [set](../../../../../set-split.md) supplies every finite increasing chain. This preparatory step uses no [Ramsey theorem](../../../../../ramsey-theorem.md).

For a finite subset $F=\{i_1<\cdots<i_r\}$ of $I$, define the [ultrafilter](../../../../../ultrafilter.md) $\mathcal U_F$ on $\mathbb N^F$ by nested membership, in this order:

$$
E\in\mathcal U_F\quad\Longleftrightarrow\quad(\mathcal U n_{i_1})\cdots(\mathcal U n_{i_r})\,[\mathbf n\in E],
$$

where $(\mathcal U n)\,Q(n)$ means $\{n:Q(n)\}\in\mathcal U$. This is the ordered [Fubini product of ultrafilters](../../../../../fubini-product-of-ultrafilters.md). Closure under intersections and the decision between a [set](../../../../../set-split.md) and its complement hold at each nested level, proving it is an [ultrafilter](../../../../../ultrafilter.md). For $F=\varnothing$ take the [principal ultrafilter](../../../../../principal-ultrafilter.md) on the one-point product. Put

$$
N_F=M_0^{\mathbb N^F}/\mathcal U_F.
$$

If $F\subseteq G$, pull a [function](../../../../../function-split.md) back along the projection $\mathbb N^G\to\mathbb N^F$. A test independent of an omitted coordinate is unchanged by its [ultrafilter](../../../../../ultrafilter.md) quantifier, so projection pushes $\mathcal U_G$ to $\mathcal U_F$. The induced map $N_F\to N_G$ is therefore an [elementary embedding](../../../../../elementary-embedding.md) by [Łoś theorem](../../../../../los-theorem.md). These maps are coherent, giving a directed system indexed by finite subsets of $I$.

Take its [directed limit of elementary embeddings](../../../../../directed-limit-of-elementary-embeddings.md) $N$. One can verify elementarity directly: representatives of a finite tuple occur at a common stage; [functions](../../../../../function-split.md) and atomic relations are interpreted there. In the existential step, a witness in the limit occurs with the parameters at some later common stage, and elementarity pulls the existence statement back. Thus every $N_F$ embeds elementarily into $N$, which contains an elementary copy of $M^+$.

For $i\in F$, let $a_i$ be the class of the coordinate [function](../../../../../function-split.md) $\mathbf n\mapsto b_{n_i}$. Projection coherence makes this independent of $F$. If $i<j$, then for each fixed $n_i$ the [set](../../../../../set-split.md) $\{n_j:n_j\ne n_i\}$ is cofinite. The nested test therefore gives $a_i\ne a_j$. In the ordered variant, the same argument with $n_j>n_i$ gives $P(a_i)$ and $a_i<a_j$.

For every [first-order formula](../../../../../first-order-formula.md) $\varphi$ of the expanded language and every increasing tuple $i_1<\cdots<i_r$, [Łoś theorem](../../../../../los-theorem.md) gives

$$
N\models\varphi(a_{i_1},\ldots,a_{i_r})\quad\Longleftrightarrow\quad(\mathcal U n_1)\cdots(\mathcal U n_r)\,[M_0\models\varphi(b_{n_1},\ldots,b_{n_r})].
$$

The right-hand side depends on the [first-order formula](../../../../../first-order-formula.md) and tuple length, not on the indices. This proves order indiscernibility in the expanded language. Let $H$ be the [Skolem hull](../../../../../skolem-hull.md) of the generators in $N$. The [Tarski-Vaught test](../../../../../tarski-vaught-test.md) gives $H\prec N$, and its reduct is a [first-order model](../../../../../model-of-a-first-order-theory.md) of $\operatorname{Th}(M)$.

An [order automorphism](../../../../../order-automorphism.md) $\pi$ of $I$ acts by

$$
t(a_{i_1},\ldots,a_{i_r})\longmapsto t(a_{\pi(i_1)},\ldots,a_{\pi(i_r)}).
$$

Indiscernibility makes this well defined: combine the finite supports of two term expressions into one increasing tuple, and apply indiscernibility to their [logical equality](../../../../../logical-equality.md). Applying it to relation [first-order formulas](../../../../../first-order-formula.md) proves preservation of all relations; the inverse is induced by $\pi^{-1}$. Every element of the hull is such a term, so the extension is unique among [structure automorphisms](../../../../../automorphism-of-a-first-order-structure.md) preserving the [Skolem expansion](../../../../../skolem-expansion.md). Moreover

$$
\boxed{|H|\leq\max(|I|,|L|,\aleph_0),\quad\text{and }|H|=|I|\text{ if }|I|\geq|L|+\aleph_0.}
$$

This proves the theorem, including its ordered version and [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md) conclusion, using [ultrapowers](../../../../../ultrapower.md) and a directed limit throughout.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
