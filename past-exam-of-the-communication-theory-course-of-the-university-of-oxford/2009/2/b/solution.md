<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every internal node of an optimal binary prefix tree has two children. If one had only one child, remove that one-edge detour from all descendant words. Prefix-freeness is preserved and at least one positive-[probability](../../../../probability.md) word becomes shorter, strictly lowering the expected length. Thus the tree is full.

Take a leaf at maximum depth $L$. Its sibling exists because the tree is full. That sibling cannot be an internal node, since a descendant would be deeper than $L$. Hence it is another leaf at depth $L$, and the corresponding codewords differ only in their final bit. This is the [deepest sibling property of an optimal prefix code](../../../../deepest-sibling-property-of-an-optimal-prefix-code.md).

A finite full binary tree satisfies [Kraft equality](../../../../kraft-mcmillan-inequality.md), $\sum_x2^{-\ell_x}=1$, by dividing mass equally down each branch from the root. If all $2^n$ lengths were at least $n$, with at least one strictly greater, that sum would be less than $2^n2^{-n}=1$, a contradiction. Since the code is not a [block code](../../../../block-code.md), the alternative that all lengths equal $n$ is excluded. Therefore **some word has length below $n$**. Also a longest word must have length above $n$: if all lengths were at most $n$ and some shorter, the Kraft sum would exceed one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
