<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a finite generating set $S$, the [Følner condition](../../../../../../folner-condition.md) requires that for every $\varepsilon>0$ there be a nonempty finite $F\subseteq G$ such that

$$
\frac{|sF\mathbin\triangle F|}{|F|}<\varepsilon
\qquad(s\in S),
$$

where $\mathbin\triangle$ denotes [symmetric difference](../../../../../../symmetric-difference.md). Choose a [Følner sequence](../../../../../../folner-sequence.md) $(F_n)$ and define normalized counting functions on all subsets $A\subseteq G$ by

$$
\mu_n(A)=\frac{|A\cap F_n|}{|F_n|}.
$$

By compactness of the product $[0,1]^{\mathcal P(G)}$, some subnet converges pointwise to a function $m$. The identities $\mu_n(G)=1$ and finite additivity on disjoint subsets pass to the limit, so $m$ is a [finitely additive probability measure](../../../../../../finitely-additive-probability-measure.md).

For a fixed $g=s_1\cdots s_\ell$, the triangle inequality for symmetric differences gives

$$
\frac{|gF_n\mathbin\triangle F_n|}{|F_n|}
\leq\sum_{j=1}^{\ell}
\frac{|s_jF_n\mathbin\triangle F_n|}{|F_n|}\longrightarrow0.
$$

Consequently

$$
|\mu_n(gA)-\mu_n(A)|
\leq\frac{|g^{-1}F_n\mathbin\triangle F_n|}{|F_n|}\longrightarrow0,
$$

so $m(gA)=m(A)$. The limit is left invariant and the [Følner condition implies amenability](../../../../../../folner-condition-implies-amenability.md). Thus **every finitely generated group satisfying the Følner condition is amenable**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 143](../../../paper-143-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
