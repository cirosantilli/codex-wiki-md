<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**The [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md).** For an [antichain](../../../../../antichain.md) $\mathcal F$ in the [Boolean lattice](../../../../../boolean-lattice.md),

$$
\boxed{\sum_{F\in\mathcal F}\binom n{|F|}^{-1}\leq1.}
$$

To prove this by [double counting](../../../../../double-counting-proof-technique.md), generate a [maximal chain in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) from a [permutation](../../../../../permutation.md) $\pi$ of $[n]$: its members are the first $j$ entries of $\pi$, for $0\leq j\leq n$. A particular $j$-set belongs to exactly $j!(n-j)!$ of the $n!$ resulting [maximal chains in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md). Each such [maximal chain in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) meets the [antichain](../../../../../antichain.md) at most once. Counting pairs consisting of a member of $\mathcal F$ and a [permutation](../../../../../permutation.md) whose associated [maximal chain in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) contains it gives

$$
\sum_{F\in\mathcal F}|F|!(n-|F|)!\leq n!.
$$

Division by $n!$ proves the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md), including the empty [antichain](../../../../../antichain.md) and the levels containing $\varnothing$ or $[n]$.

**A [symmetric chain decomposition of a Boolean lattice](../../../../../symmetric-chain-decomposition-of-a-boolean-lattice.md).** A [symmetric chain](../../../../../symmetric-chain-in-a-boolean-lattice.md) has one set at every size from $k$ to $n-k$, with consecutive members related by inclusion. Start with the single [symmetric chain](../../../../../symmetric-chain-in-a-boolean-lattice.md) containing $\varnothing$ when $n=0$. Given a [symmetric chain](../../../../../symmetric-chain-in-a-boolean-lattice.md)

$$
A_k\subset A_{k+1}\subset\cdots\subset A_{n-k}
$$

in a [symmetric chain decomposition of a Boolean lattice](../../../../../symmetric-chain-decomposition-of-a-boolean-lattice.md) on $[n]$, let $x=n+1$ and replace its two copies in the larger [Boolean lattice](../../../../../boolean-lattice.md) by

$$
A_k\subset\cdots\subset A_{n-k}\subset A_{n-k}\cup\{x\},
$$

and, when it is nonempty, by

$$
A_k\cup\{x\}\subset\cdots\subset A_{n-k-1}\cup\{x\}.
$$

The endpoint sizes of the first [symmetric chain](../../../../../symmetric-chain-in-a-boolean-lattice.md) sum to $n+1$; those of the second [symmetric chain](../../../../../symmetric-chain-in-a-boolean-lattice.md) also sum to $n+1$. These [symmetric chains](../../../../../symmetric-chain-in-a-boolean-lattice.md) partition the original [symmetric chain](../../../../../symmetric-chain-in-a-boolean-lattice.md) together with its copy containing $x$. Thus this construction inductively partitions the entire [Boolean lattice](../../../../../boolean-lattice.md) into [symmetric chains](../../../../../symmetric-chain-in-a-boolean-lattice.md). Each [symmetric chain](../../../../../symmetric-chain-in-a-boolean-lattice.md) contains exactly one set of size $\lfloor n/2\rfloor$, so the number of [symmetric chains](../../../../../symmetric-chain-in-a-boolean-lattice.md) is

$$
\boxed{\binom n{\lfloor n/2\rfloor}.}
$$

**The proposed sum bound for [cross-intersecting families](../../../../../cross-intersecting-family.md) is false.** Take $n=3$ and

$$
\mathcal A=\mathcal B=\bigl\{\{1,2\},\{1,3\},\{2,3\}\bigr\}.
$$

Both are [antichains](../../../../../antichain.md), and any member of one meets any member of the other. Nevertheless,

$$
\boxed{|\mathcal A|+|\mathcal B|=6>3=\binom3{\lfloor3/2\rfloor}.}
$$

The hypothesis permits the two [antichains](../../../../../antichain.md) to coincide. Even if distinct [antichains](../../../../../antichain.md) were wanted, taking $\mathcal B=\{\{1,2\},\{1,3\}\}$ gives $5>3$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
