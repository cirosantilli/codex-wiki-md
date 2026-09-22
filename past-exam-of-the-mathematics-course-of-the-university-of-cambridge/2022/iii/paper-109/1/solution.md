<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $\mathcal A\subseteq[n]^{(r)}$, the [Local LYM inequality](../../../../../local-lym-inequality.md) is

$$
\frac{|\partial\mathcal A|}{\binom n{r-1}}
\geq
\frac{|\mathcal A|}{\binom nr}.
$$

Count containment pairs $(B,A)$ with $B\in\partial\mathcal A$, $A\in\mathcal A$, and $B\subset A$. Every $A$ contributes $r$ pairs, while every $B$ contributes at most $n-r+1$. Hence

$$
r|\mathcal A|\leq(n-r+1)|\partial\mathcal A|,
$$

which rearranges to the claimed normalized inequality.

The [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) says that every [antichain](../../../../../antichain.md) $\mathcal F\subseteq\mathcal P([n])$ satisfies

$$
\boxed{\sum_{A\in\mathcal F}\binom n{|A|}^{-1}\leq1.}
$$

For the local-LYM proof, replace the highest nonempty level of $\mathcal F$ by its lower shadow. No shadow member contains a surviving member, since that would make the original family non-antichain, and the local inequality says that the normalized size does not decrease. Repeating pushes the family to the bottom level, whose normalized size is at most one. Therefore the original normalized sum was at most one.

For the chain proof, choose a [Uniformly random maximal chain in a Boolean lattice](../../../../../uniformly-random-maximal-chain-in-a-boolean-lattice.md). A fixed $r$-set belongs to it with probability $\binom nr^{-1}$. Since an antichain meets each chain at most once, the expected number of its members on the chain is at most one. Linearity of expectation gives the displayed sum.

Finally use a [symmetric chain decomposition of a Boolean lattice](../../../../../symmetric-chain-decomposition-of-a-boolean-lattice.md). Convexity makes the intersection of $\mathcal A$ with each symmetric chain an interval. The alternating sum of $(-1)^{|A|}$ over an interval in a chain is $0$, $1$, or $-1$. There are exactly $\binom n{\lfloor n/2\rfloor}$ chains, because each contains exactly one member of a middle level. Summing the chain contributions gives

$$
\boxed{
\left|\sum_{A\in\mathcal A}(-1)^{|A|}\right|
\leq\binom n{\lfloor n/2\rfloor}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
