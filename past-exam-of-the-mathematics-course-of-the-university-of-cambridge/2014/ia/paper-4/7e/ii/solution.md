<h1 id="7e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $\mathbb N=\{1,2,\ldots\}$. If a [bijection](../../../../../../bijection.md) $f:\mathbb N\to\mathbb N$ maps $S$ onto the even [natural numbers](../../../../../../natural-number.md), its restriction is a [bijection](../../../../../../bijection.md) from $S$ onto an infinite [set](../../../../../../set-split.md). Moreover, its restriction to the [complement](../../../../../../complement-of-a-set.md) of $S$ maps onto the odd [natural numbers](../../../../../../natural-number.md). Both [sets](../../../../../../set-split.md) are therefore infinite.

Conversely, suppose that $S$ and its [complement](../../../../../../complement-of-a-set.md) are infinite. Applying the [increasing enumeration of an infinite subset of natural numbers](../../../../../../increasing-enumeration-of-an-infinite-subset-of-natural-numbers.md) to each gives

$$
S=\{s_1<s_2<\cdots\},\qquad\mathbb N\setminus S=\{t_1<t_2<\cdots\}.
$$

For completeness, successively choose the least unused member. The process never stops because the [set](../../../../../../set-split.md) is infinite, and it lists every member: an omitted member would have infinitely many selected [natural numbers](../../../../../../natural-number.md) below it, which is impossible. Define

$$
\boxed{f(s_j)=2j,\qquad f(t_j)=2j-1.}
$$

This is [injective](../../../../../../injective-function.md) on each list, their images are disjoint, and together their images cover $\mathbb N$. Thus it is a [bijection](../../../../../../bijection.md) and maps $S$ onto $2\mathbb N$. **Both infinitude conditions are necessary and sufficient.** If a convention includes zero in $\mathbb N$, index each list from zero and use $2j$, $2j+1$ instead.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [7E](../../7e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
