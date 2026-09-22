<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the following [decision-tree adversary for a threshold function](../../../../../../decision-tree-adversary-for-a-threshold-function.md). Regardless of which variables the tree queries, answer $0$ on the first $n-r$ queries and $1$ on the next $r-1$ queries. After any proper prefix of this answer sequence, the unqueried variables can be completed both to an input of weight below $r$ and to one of weight at least $r$. Immediately before the last query the answers contain exactly $n-r$ zeros and $r-1$ ones, so the final bit alone determines the value of the [Threshold Boolean function](../../../../../../threshold-function.md) $f_{n,r}$. Thus every decision tree has a root-to-leaf path of length $n$, while querying all variables gives depth $n$. Hence

$$
\boxed{D(f_{n,r})=n.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
