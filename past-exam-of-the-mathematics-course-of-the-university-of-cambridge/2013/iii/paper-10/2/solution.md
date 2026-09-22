<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The **[Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md)** states that a [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) minimizes the [lower shadow](../../../../../lower-shadow.md) of a [uniform set family](../../../../../uniform-set-family.md) of prescribed size. Its numerical form is as follows. For $m>0$, write the unique [combinatorial number system](../../../../../combinatorial-number-system.md) expansion

$$
m=\binom{a_r}r+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_s}s,\qquad a_r>a_{r-1}>\cdots>a_s\geq s\geq1.
$$

Every $\mathcal F\subseteq[n]^{(r)}$ of size $m$ satisfies

$$
\boxed{|\partial\mathcal F|\geq\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_s}{s-1}}.
$$

The empty family has empty [lower shadow](../../../../../lower-shadow.md). Equality is attained by the first $m$ $r$-sets in [colexicographic order](../../../../../colexicographic-order.md), where the largest differing element belongs to the later set. Iterating the [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) shows that the same [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) minimizes every [iterated lower shadow](../../../../../iterated-lower-shadow.md).

For $1\leq r<n/2$, the **[Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md)** gives

$$
\boxed{|\mathcal F|\leq\binom{n-1}{r-1}}
$$

for an [intersecting family](../../../../../intersecting-family.md) $\mathcal F\subseteq[n]^{(r)}$. All $r$-sets containing one prescribed point show that the bound is sharp.

For the proof from the [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md), put $k=n-r$ and form the complement family $\mathcal G=\{[n]\setminus A:A\in\mathcal F\}\subseteq[n]^{(k)}$. Let $\mathcal S$ be its rank-$r$ [iterated lower shadow](../../../../../iterated-lower-shadow.md). No member $B\in\mathcal F$ belongs to $\mathcal S$: containment in $[n]\setminus A$ would give $A\cap B=\varnothing$, impossible for an [intersecting family](../../../../../intersecting-family.md) of nonempty sets. Hence

$$
|\mathcal F|+|\mathcal S|\leq\binom nr.
$$

Suppose $|\mathcal F|>\binom{n-1}{r-1}=\binom{n-1}k$. The first $\binom{n-1}k$ members of the [colexicographic order](../../../../../colexicographic-order.md) are all $k$-sets of $[n-1]$. Their rank-$r$ [iterated lower shadow](../../../../../iterated-lower-shadow.md) is all $r$-sets of $[n-1]$, since $r<k$. The next $k$-set contains $n$ and has an $r$-subset containing $n$, so taking even one more member strictly enlarges that [iterated lower shadow](../../../../../iterated-lower-shadow.md). By the iterated [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md), $|\mathcal S|>\binom{n-1}r$. Together with $|\mathcal F|>\binom{n-1}{r-1}$ this contradicts [Pascal's identity](../../../../../pascal-s-rule.md) and the preceding inequality. This proves the [Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md).

For the [Katona circle method](../../../../../katona-circle-method.md) proof, fix a [cyclic ordering](../../../../../cyclic-ordering.md) of $[n]$. A [cyclic interval](../../../../../cyclic-interval.md) of length $r$ is specified by its final position. If no such interval belongs to $\mathcal F$, the bound below is automatic. Otherwise rotate one selected interval so that it ends at position $n$, and thus occupies positions $n-r+1,\ldots,n$. Intervals ending at positions $r,\ldots,n-r$ are disjoint from it and cannot be selected. Among the remaining endpoints, pair $j$ with $n-r+j$ for $1\leq j\leq r-1$. The corresponding intervals are disjoint when $n\geq2r$, so at most one interval per pair is selected. Together with the interval ending at $n$, this gives the [cyclic interval intersection bound](../../../../../cyclic-interval-intersection-bound.md) of $r$ selected intervals.

Choose a uniformly random [permutation](../../../../../permutation.md) and read its positions cyclically. A fixed $r$-set is a [cyclic interval](../../../../../cyclic-interval.md) with probability $n/\binom nr$: each cyclic position gives a uniformly distributed $r$-set, and for $r<n$ the $n$ intervals are distinct. Summing over $\mathcal F$, the [expected value](../../../../../expected-value.md) of the number of selected intervals is $n|\mathcal F|/\binom nr$. The [cyclic interval intersection bound](../../../../../cyclic-interval-intersection-bound.md) makes this at most $r$, giving $|\mathcal F|\leq(r/n)\binom nr=\binom{n-1}{r-1}$.

Finally apply the [Katona circle method](../../../../../katona-circle-method.md) to an arbitrary [antichain](../../../../../antichain.md) $\mathcal A$. If it contains $\varnothing$ or $[n]$, it has exactly one member and the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) holds with equality. Otherwise all its members have sizes $1,\ldots,n-1$. In a fixed [cyclic ordering](../../../../../cyclic-ordering.md), the [cyclic intervals](../../../../../cyclic-interval.md) sharing a final position form a nested chain as their lengths increase. At most one of them can belong to the [antichain](../../../../../antichain.md). Summing over the $n$ final positions proves the [cyclic interval antichain bound](../../../../../cyclic-interval-antichain-bound.md) of $n$ intervals. Taking the [expected value](../../../../../expected-value.md) over a uniformly random [permutation](../../../../../permutation.md) gives

$$
n\sum_{r=1}^{n-1}\frac{|\mathcal A\cap[n]^{(r)}|}{\binom nr}\leq n.
$$

After division by $n$, this is **the [LYM inequality](../../../../../lubell-yamamoto-meshalkin-inequality.md) proved by cyclic intervals**. The case $n=0$ consists only of the empty set and is immediate.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
