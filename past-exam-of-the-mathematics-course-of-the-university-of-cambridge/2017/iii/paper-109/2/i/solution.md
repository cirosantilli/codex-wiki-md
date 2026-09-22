<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The sharp bound form of the [Erdős-Ko-Rado theorem](../../../../../../erdos-ko-rado-theorem.md) is as follows. If $1\leq r\leq n/2$ and $\mathcal F\subseteq\binom{[n]}r$ is an [intersecting family](../../../../../../intersecting-family.md), then

$$
\boxed{|\mathcal F|\leq\binom{n-1}{r-1}.}
$$

The [uniform set family](../../../../../../uniform-set-family.md) of all $r$-element [subsets](../../../../../../subset.md) containing one fixed point attains the bound. We prove it by the [Katona circle method](../../../../../../katona-circle-method.md).

First establish the [cyclic interval intersection bound](../../../../../../cyclic-interval-intersection-bound.md). In any fixed cyclic ordering of $[n]$, at most $r$ cyclic intervals of length $r$ can form an [intersecting family](../../../../../../intersecting-family.md). If there is a selected interval, rotate the ordering so that it ends at position $n$ and consists of positions $n-r+1,\ldots,n$. Intervals ending at positions $r,\ldots,n-r$ are disjoint from it and cannot be selected. Of the remaining intervals, one ends at $n$; the others have endpoints paired as

$$
(j,\ j+n-r),\qquad 1\leq j\leq r-1.
$$

The two intervals in each pair are disjoint: one wraps around position $n$ and the other lies in the intervening gap, since $n\geq2r$. At most one of each pair belongs to the [intersecting family](../../../../../../intersecting-family.md), giving at most $1+(r-1)=r$ intervals.

Now count pairs $(\sigma,A)$ where $\sigma$ is a [permutation](../../../../../../permutation.md) of $[n]$ placed on labelled cyclic positions and $A\in\mathcal F$ occupies $r$ consecutive positions. Each [permutation](../../../../../../permutation.md) contributes at most $r$ pairs by the [cyclic interval intersection bound](../../../../../../cyclic-interval-intersection-bound.md). Each fixed $A$ contributes $n\,r!\,(n-r)!$ pairs: choose its starting position and order the elements inside and outside its interval. Since $r<n$, the starting position is unique for each such placement. Consequently

$$
|\mathcal F|\,n\,r!\,(n-r)!\leq r\,n!,\qquad |\mathcal F|\leq\frac{r}{n}\binom nr=\binom{n-1}{r-1}.
$$

This completes the [Erdős-Ko-Rado theorem](../../../../../../erdos-ko-rado-theorem.md) proof. At $n=2r$, complementary $r$-element [subsets](../../../../../../subset.md) are the only disjoint pairs, so choosing one member of every complementary pair gives an extremiser. This describes all equality cases at that boundary. The range $n\geq2r$ is essential: for $n<2r$, the entire [uniform set family](../../../../../../uniform-set-family.md) is an [intersecting family](../../../../../../intersecting-family.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
