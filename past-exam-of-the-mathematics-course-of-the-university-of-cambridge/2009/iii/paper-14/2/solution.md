<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md) asserts that, for $1\leq r<n/2$, every [intersecting family](../../../../../intersecting-family.md) $\mathcal A\subseteq\binom{[n]}r$ satisfies

$$
\boxed{|\mathcal A|\leq\binom{n-1}{r-1}.}
$$

The bound is attained by the [set family](../../../../../set-family.md) of all $r$-subsets containing one prescribed point. Here [lexicographic order](../../../../../lexicographic-order.md) means that $X<Y$ when the smallest element of their [symmetric difference](../../../../../symmetric-difference.md) belongs to $X$.

The first $M=\binom{n-1}{r-1}$ members in [lexicographic order](../../../../../lexicographic-order.md) are exactly those containing $1$. An initial segment longer than $M$ contains all of them and also the first member avoiding $1$, namely $B=\{2,\ldots,r+1\}$. There is an $r$-subset containing $1$ and disjoint from $B$: choose its other $r-1$ elements from $\{r+2,\ldots,n\}$, which has $n-r-1\geq r-1$ elements. Consequently any longer [lexicographic](../../../../../lexicographic-order.md) initial segment fails to be an [intersecting family](../../../../../intersecting-family.md). Thus preservation of the [intersection](../../../../../set-intersection.md) property upon replacing a [set family](../../../../../set-family.md) by the equally large [lexicographic](../../../../../lexicographic-order.md) initial segment proves the displayed bound.

Here is a direct [UV-compression](../../../../../uv-compression.md) proof of that preservation statement. For disjoint nonempty [sets](../../../../../set-split.md) $U,V$ with $|U|=|V|$ and $\min U<\min V$, an eligible member $A$ contains $V$ and misses $U$; its proposed image is $A'=(A\setminus V)\cup U$. The [UV-compression](../../../../../uv-compression.md) moves $A$ to $A'$ only if $A'$ is not already present. Each eligible pair is either kept as a pair or moved from its later to its earlier member, so this operation preserves cardinality and uniformity and strictly decreases the sum of [lexicographic order](../../../../../lexicographic-order.md) positions whenever it changes the [set family](../../../../../set-family.md).

The essential [intersection-preserving lexicographic UV-compression](../../../../../intersection-preserving-lexicographic-uv-compression.md) lemma is that this operation preserves an [intersecting family](../../../../../intersecting-family.md) whenever all smaller lexicographically improving [UV-compressions](../../../../../uv-compression.md) already leave that [set family](../../../../../set-family.md) unchanged. Suppose instead that the compressed [set family](../../../../../set-family.md) has disjoint members. At least one, say $A'$, must be newly moved. Both newly moved members would contain $U$, so the other, $B$, is a retained old member. Write $A=(A'\setminus U)\cup V$ for the old preimage. Since $A'\cap B=\varnothing$, we have $B\cap U=\varnothing$ and $(A\setminus V)\cap B=\varnothing$. Old intersectingness forces

$$
V'=V\cap B\ne\varnothing.
$$

If $V'=V$, then $B$ was eligible for the same [UV-compression](../../../../../uv-compression.md). Since it was retained, $B'=(B\setminus V)\cup U$ was already present. But $A\cap B'=\varnothing$, contradicting old intersectingness.

Otherwise $0<|V'|<|V|$. Choose $U'\subset U$ with $|U'|=|V'|$ and $\min U\in U'$. This is a smaller improving pair, since $\min U'=\min U<\min V\leq\min V'$. The old member $A$ is eligible for its [UV-compression](../../../../../uv-compression.md). The assumed stability therefore forces $A''=(A\setminus V')\cup U'$ to be present already. Yet its portion outside $V$ misses $B$, its remaining portion $V\setminus V'$ misses $B$, and $U'$ misses $B$. Thus $A''\cap B=\varnothing$, the required contradiction. This proves the lemma, including the size-one case, where only the first alternative can arise.

Starting with $\mathcal A$, repeatedly choose a changing improving [UV-compression](../../../../../uv-compression.md) with the smallest possible $|U|$. The lemma applies at each step because every smaller improving [UV-compression](../../../../../uv-compression.md) is then unchanged. Thus every intermediate [set family](../../../../../set-family.md) is intersecting. The strictly decreasing nonnegative integer sum of [lexicographic order](../../../../../lexicographic-order.md) positions ensures termination. If the terminal [set family](../../../../../set-family.md) were not an initial segment, there would be a missing $X$ earlier than a present $Y$. Taking $U=X\setminus Y$ and $V=Y\setminus X$ gives equally sized nonempty disjoint [sets](../../../../../set-split.md) with $\min U<\min V$, and moves $Y$ to the missing $X$. That contradicts termination. The terminal [set family](../../../../../set-family.md) is therefore exactly the equally large [lexicographic](../../../../../lexicographic-order.md) initial segment, and it is intersecting. **This proves the required lexicographic statement directly, and hence the [Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md).**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
