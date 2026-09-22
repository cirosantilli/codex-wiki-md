# Equal-or-disjoint translates characterize cosets

↑ **Parent:** [Coset](coset.md)

A nonempty [subset](subset.md) $B$ of any [group](group-split.md) $G$ is a [left coset](left-coset.md) of a [subgroup](subgroup.md) if and only if any two left translates $gB,hB$ are equal or disjoint. No finiteness assumption is needed.

For the forward direction, write $B=bH$ with $H$ a [subgroup](subgroup.md). Then $gB=gbH$, and distinct [left cosets](left-coset.md) of $H$ are disjoint. For the converse, first assume $e\in B$. For every $b\in B$, $b\in B\cap bB$, so $bB=B$. This proves closure under multiplication. Since $e\in B=bB$, there is $c\in B$ with $bc=e$, showing $b^{-1}\in B$. Thus $B$ passes the [subgroup test](subgroup-test.md).

For a general nonempty $B$, choose $b\in B$ and set $H=b^{-1}B$. It contains $e$, and all its left translates have the assumed property because $gH=(gb^{-1})B$. The previous argument makes $H$ a [subgroup](subgroup.md), and $B=bH$ is a [left coset](left-coset.md). This gives a recognition criterion for [cosets](coset.md) from their translate intersections alone.

## ↑ Ancestors (6)

1. [Coset](coset.md)
2. [Group theory](group-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-i/5/b/ii/solution.md)
