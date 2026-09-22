<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Erdős-Ko-Rado theorem](../../../../../../erdos-ko-rado-theorem.md) states that for $1\le r\le n/2$, an [intersecting family](../../../../../../intersecting-family.md) $\mathcal F$ of $r$-subsets of $[n]$ satisfies

$$
\boxed{|\mathcal F|\le\binom{n-1}{r-1}}.
$$

The bound is sharp: take all $r$-sets containing one fixed element.

Use the [Katona circle method](../../../../../../katona-circle-method.md). In any cyclic ordering of $[n]$, the [cyclic interval intersection bound](../../../../../../cyclic-interval-intersection-bound.md) permits at most $r$ members of $\mathcal F$ to appear as length-$r$ intervals. To see the bound directly, rotate a chosen interval so that it ends at $n$. Intervals ending at $r,\ldots,n-r$ miss it. Pair the remaining endpoints except $n$ as $(j,j+n-r)$, $1\le j\le r-1$; the two intervals in each pair are disjoint, so at most one is chosen. Including the fixed interval gives at most $r$.

There are $(n-1)!$ oriented cyclic orders. A fixed $r$-set appears consecutively in $r!(n-r)!$ of them: collapse it to a block, cyclically order that block with the other $n-r$ elements, and order its members internally. [Double counting](../../../../../../double-counting-proof-technique.md) the compatible family-member/order pairs gives $|\mathcal F|r!(n-r)!\le r(n-1)!$, proving the theorem.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
