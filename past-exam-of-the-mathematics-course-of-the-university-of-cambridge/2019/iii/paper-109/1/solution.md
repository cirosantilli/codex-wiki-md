<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [uniform set family](../../../../../uniform-set-family.md) $\mathcal A\subseteq[n]^{(r)}$, the [Local LYM inequality](../../../../../local-lym-inequality.md) is

$$
\frac{|\partial\mathcal A|}{\binom n{r-1}}
\geq
\frac{|\mathcal A|}{\binom nr}.
$$

To prove it, count the incident pairs $(B,A)$ with $B\in\partial\mathcal A$, $A\in\mathcal A$, and $B\subset A$. Every $A$ contributes exactly $r$ pairs, whereas every $B$ belongs to at most $n-r+1$ members of $[n]^{(r)}$. Therefore

$$
r|\mathcal A|\leq(n-r+1)|\partial\mathcal A|,
$$

which is the displayed inequality after using the [binomial coefficient](../../../../../binomial-coefficient.md) identity $r\binom nr=(n-r+1)\binom n{r-1}$.

The [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) says that every [antichain](../../../../../antichain.md) $\mathcal A\subseteq\mathcal P([n])$ satisfies

$$
\boxed{\displaystyle \sum_{A\in\mathcal A}\binom n{|A|}^{-1}\leq1.}
$$

For the proof from the local inequality, take the lowest occupied level below the middle and replace that level by its [upper shadow](../../../../../upper-shadow.md). The result remains an [antichain](../../../../../antichain.md): any new containment involving a set in the upper shadow would already give a containment involving the member of $\mathcal A$ immediately below it. The dual form of the [Local LYM inequality](../../../../../local-lym-inequality.md) says that this replacement cannot decrease the [Lubell mass](../../../../../lubell-mass.md). Repeating upward below the middle, and similarly replacing high levels by their [lower shadows](../../../../../lower-shadow.md), eventually puts the whole family in one middle level. Its final Lubell mass is at most one, so the original mass is also at most one.

For the [maximal chain in a Boolean lattice](../../../../../maximal-chain-in-a-boolean-lattice.md) proof, choose a [Uniformly random maximal chain in a Boolean lattice](../../../../../uniformly-random-maximal-chain-in-a-boolean-lattice.md). An $h$-element set lies on it with [probability](../../../../../probability.md) $1/\binom nh$. Because an [antichain](../../../../../antichain.md) meets each chain at most once, the [expected value](../../../../../expected-value.md) of the number of its members on the chain is at most one. By [linearity of expectation](../../../../../linearity-of-expectation.md), that expected value is precisely the displayed sum.

The [Sperner theorem](../../../../../sperner-s-theorem.md) follows because $\binom n{|A|}\leq\binom n{\lfloor n/2\rfloor}$ for every $A$. If equality holds in the resulting cardinality bound, every member lies on a largest level. For even $n$ this is the unique middle level. For odd $n$, the two middle levels have equal size; the regular connected inclusion graph between them and equality in [Local LYM inequality](../../../../../local-lym-inequality.md) force a chosen portion of the lower level to be either empty or the whole level. Hence the maximum [antichains](../../../../../antichain.md) are **exactly the complete middle level, with either middle level allowed when $n$ is odd**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
