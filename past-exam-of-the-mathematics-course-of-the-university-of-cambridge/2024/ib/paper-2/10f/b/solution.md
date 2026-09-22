<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X$ be compact Hausdorff, let $x\in X$, and let $U$ be a neighbourhood of $x$. Choose an open $O$ with $x\in O\subseteq U$. Apply the separation result from part (a) to the disjoint closed sets $\{x\}$ and $X\setminus O$. There is an open $V\ni x$ whose closure lies in $O$. Then

$$
K=\overline V
$$

is compact, contains the neighbourhood $V$ of $x$, and lies in $U$. Thus $X$ is locally compact.

Conversely, suppose $X$ is locally compact Hausdorff and $A\cap K$ is closed in every compact $K\subseteq X$. For $x\notin A$, choose a compact neighbourhood $K$ of $x$ and an [open set](../../../../../../open-set.md) $U$ with

$$
x\in U\subseteq K.
$$

Since $A\cap K$ is closed in $K$, there is an [open set](../../../../../../open-set.md) $W\subseteq X$ such that

$$
K\setminus(A\cap K)=K\cap W.
$$

Then $U\cap W$ is an open neighbourhood of $x$ disjoint from $A$. Thus $X\setminus A$ is open and

$$
\boxed{A\text{ is closed}}.
$$

This is the [compactly detected closed-set theorem in a locally compact Hausdorff space](../../../../../../compactly-detected-closed-set-theorem-in-a-locally-compact-hausdorff-space.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
