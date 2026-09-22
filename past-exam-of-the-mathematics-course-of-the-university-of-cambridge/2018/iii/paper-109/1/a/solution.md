<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a [Uniformly random maximal chain in a Boolean lattice](../../../../../../uniformly-random-maximal-chain-in-a-boolean-lattice.md) by taking a uniformly random [permutation](../../../../../../permutation.md) of $X$ and successively adjoining its elements. A fixed $r$-element set occurs on this [maximal chain in a Boolean lattice](../../../../../../maximal-chain-in-a-boolean-lattice.md) with probability $r!(n-r)!/n!=\binom nr^{-1}$. Because an [antichain](../../../../../../antichain.md) meets every such [chain in a partially ordered set](../../../../../../chain-in-a-partially-ordered-set.md) at most once, [linearity of expectation](../../../../../../linearity-of-expectation.md) gives the [LYM inequality](../../../../../../lubell-yamamoto-meshalkin-inequality.md):

$$
L(\mathcal A):=\sum_{A\in\mathcal A}\binom n{|A|}^{-1}=\mathbb E|\mathcal A\cap\mathcal C|\leq1.
$$

Here $L(\mathcal A)$ is the [Lubell mass](../../../../../../lubell-mass.md).

For [equality in the LYM inequality](../../../../../../equality-in-the-lym-inequality.md), the integer $|\mathcal A\cap\mathcal C|\leq1$ must equal one for every [maximal chain in a Boolean lattice](../../../../../../maximal-chain-in-a-boolean-lattice.md), since every chain has positive probability. Choose $A\in\mathcal A$ of rank $r$. If $0<r<n$, take $x\in A$ and $y\notin A$, and choose a [permutation](../../../../../../permutation.md) with its first $r$ elements equal to $A$, its $r$th element $x$, and its next element $y$. Interchanging those two adjacent elements changes precisely the rank-$r$ member of the corresponding [maximal chain in a Boolean lattice](../../../../../../maximal-chain-in-a-boolean-lattice.md), replacing $A$ by $A'=A\setminus\{x\}\cup\{y\}$. All other members are unchanged and none belongs to the [antichain](../../../../../../antichain.md). The new chain must still meet $\mathcal A$, so $A'\in\mathcal A$.

Successive exchanges connect all $r$-element subsets: exchange an element outside a desired target for an element missing from it, decreasing the number of differences each time. Thus $\mathcal A$ contains the whole rank-$r$ level. Every set of another rank is comparable with some set in that level, so the [antichain](../../../../../../antichain.md) contains nothing else. If $r=0$ or $r=n$, its sole possible member is already the whole corresponding level. Conversely, every full level meets every [maximal chain in a Boolean lattice](../../../../../../maximal-chain-in-a-boolean-lattice.md) exactly once. Hence

$$
\boxed{L(\mathcal A)\leq1,\qquad L(\mathcal A)=1\iff\mathcal A=X^{(r)}\text{ for some }0\leq r\leq n.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
