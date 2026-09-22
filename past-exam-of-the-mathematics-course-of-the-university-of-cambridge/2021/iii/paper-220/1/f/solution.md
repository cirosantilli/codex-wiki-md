<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Choose a root $o\in T$ and finite sets $F_n\subset T$ whose union is dense, arranging that $F_n$ is a $2^{-n}$-net and $F_n\subset F_{n+1}$. Let $T_n$ be the finite subtree spanned by $o$ and $F_n$. A depth-first contour traversal of $T_n$, recording distance from $o$, gives a continuous excursion $g_n$ whose [real tree encoded by an excursion](../../../../../../real-tree-encoded-by-an-excursion.md) is $T_n$.

The traversals may be chosen compatibly: when passing from $T_n$ to $T_{n+1}$, insert the new branch traversals into small time intervals at their attachment points. Since every new component has height at most $2^{-n+1}$, choose the time changes so that

$$
\lVert g_{n+1}-g_n\rVert_\infty\leq 2^{-n+2}.
$$

After harmlessly taking a faster sequence of nets, these errors are [summable](../../../../../../summable-sequence.md). Hence $(g_n)$ is [Uniformly Cauchy](../../../../../../uniformly-cauchy-sequence.md) and converges uniformly to a continuous $g:[0,1]\to\mathbb R_+$ with $g(0)=g(1)=0$.

The net property gives $d_{GH}(T_n,T)\to0$. By the stated continuity of excursion coding, $d_{GH}(T_{g_n},T_g)\to0$. Since $T_{g_n}$ is [isometric](../../../../../../isometry.md) to $T_n$, uniqueness of limits in the [Gromov-Hausdorff distance](../../../../../../gromov-hausdorff-distance.md) implies that $T_g$ is [isometric](../../../../../../isometry.md) to $T$. This proves the [excursion coding theorem for compact real trees](../../../../../../excursion-coding-theorem-for-compact-real-trees.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 220](../../../paper-220-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
