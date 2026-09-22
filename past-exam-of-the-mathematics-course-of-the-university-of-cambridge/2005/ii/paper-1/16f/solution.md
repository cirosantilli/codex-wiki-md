<h1 id="16f/solution">Solution</h1>

↑ **Parent:** [16F](../16f.md)

[Zorn lemma](../../../../../zorn-s-lemma.md) states that a nonempty [partially ordered set](../../../../../partially-ordered-set.md) in which every chain has an upper bound contains a maximal element. To prove it from the [axiom of choice](../../../../../axiom-of-choice.md) and [Hartogs theorem](../../../../../hartogs-theorem.md), suppose no element were maximal. Fix a choice function on the nonempty subsets of the poset. Every chain then has a strict upper bound: choose an upper bound, and, since it is not maximal, choose an element strictly above it. Let $\kappa$ be a Hartogs ordinal which cannot inject into the poset. By [transfinite recursion](../../../../../transfinite-recursion.md) for $\alpha<\kappa$, choose a strict upper bound $x_\alpha$ of all previously chosen $x_\beta$, $\beta<\alpha$; for the empty initial chain choose any element. The previous elements form a chain at every stage. The resulting strictly increasing sequence injects $\kappa$ into the poset, contradicting Hartogs. Hence a maximal element exists. **Choice is used in fixing the function selecting a strict upper bound at every successor and limit stage**; Hartogs and [transfinite recursion](../../../../../transfinite-recursion.md) themselves do not supply those selections.

Apply [Zorn lemma](../../../../../zorn-s-lemma.md) to the linearly independent subsets of $\mathbb R$ over $\mathbb Q$, ordered by inclusion. A chain's union is linearly independent because any finite linear relation is contained in one member of the chain. A maximal independent set $B$ must span $\mathbb R$, since otherwise one could append a [vector](../../../../../vector.md) outside its span. Thus **$B$ is a rational-vector-space basis of $\mathbb R$**.

It is infinite: a finite-dimensional rational [vector space](../../../../../vector-space-split.md) is countable, whereas $\mathbb R$ is not. If its cardinal is $\kappa$, finite rational linear combinations show $|\mathbb R|=\max(\aleph_0,\kappa)$; uncountability forces $\kappa=|\mathbb R|$. A basis of $\mathbb R^2$ is $(B\times\{0\})\cup(\{0\}\times B)$, where these expressions mean the [vectors](../../../../../vector.md) $(b,0)$ and $(0,b)$. Its cardinal is $\kappa+\kappa=\kappa$, using the infinite-cardinal arithmetic available under choice. A bijection between the two bases extends uniquely by finite rational linear combinations to a linear bijection. Therefore

$$
\boxed{\mathbb R\cong_{\mathbb Q}\mathbb R^2.}
$$

This is an algebraic isomorphism, with no assertion of continuity or real-linearity.

## ↑ Ancestors (10)

1. [16F](../16f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
