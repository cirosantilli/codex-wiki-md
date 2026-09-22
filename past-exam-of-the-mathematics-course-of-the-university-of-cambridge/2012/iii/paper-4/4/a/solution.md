<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We use [Zorn's lemma](../../../../../../zorn-s-lemma.md), and no [basis](../../../../../../basis.md) or other existence theorem from linear algebra. A subset $B\subseteq V$ is [linearly independent](../../../../../../linear-independence.md) if every finite relation $\sum_{b\in F}\lambda_b b=0$ forces every coefficient to be zero.

Order the [linearly independent](../../../../../../linear-independence.md) subsets by inclusion. This partially ordered set is nonempty, because the empty subset is independent. An empty chain has the empty subset as an upper bound. For any nonempty chain, its union is independent: every finite subset of that union lies in one member of the chain. Indeed choose one chain member containing each of its finitely many vectors, then take the largest among that finite collection of comparable members. Every finite relation in the union is therefore a relation in an independent chain member. The union is an upper bound.

[Zorn's lemma](../../../../../../zorn-s-lemma.md) gives a maximal independent subset $B$. If $v$ were outside its span, then $B\cup\{v\}$ would still be independent. In a finite relation

$$
\lambda v+\sum_{b\in F}\lambda_b b=0,
$$

a nonzero $\lambda$ could be inverted in the [field](../../../../../../field.md) $k$, placing $v$ in the span of $B$. If $\lambda=0$, independence of $B$ forces the remaining coefficients to be zero. This contradicts maximality, so $B$ spans $V$.

Define the [free module](../../../../../../free-module.md) on $B$ as the [direct sum](../../../../../../direct-sum.md) $k^{(B)}=\bigoplus_{b\in B}k$: its elements are coefficient families with finite support. The map

$$
\Phi:k^{(B)}\longrightarrow V,\qquad(\lambda_b)\longmapsto\sum_b\lambda_b b
$$

is a module homomorphism. Spanning proves surjectivity; independence proves injectivity. Hence the [vector-space freeness from maximal independence](../../../../../../vector-space-freeness-from-maximal-independence.md) gives

$$
\boxed{V\cong\bigoplus_{b\in B}k}.
$$

Finite support is essential; this is a [direct sum](../../../../../../direct-sum.md), not an unrestricted product. The zero [vector space](../../../../../../vector-space-split.md) uses $B=\varnothing$ and is free of rank zero. The proof for arbitrary [vector spaces](../../../../../../vector-space-split.md) explicitly uses the [axiom of choice](../../../../../../axiom-of-choice.md) through [Zorn's lemma](../../../../../../zorn-s-lemma.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
