<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

Let $S$ be the [vector subspace](../../../../../../../vector-subspace.md) of [symmetric matrices](../../../../../../../symmetric-matrix.md). A [basis](../../../../../../../basis.md) consists of $E_{ii}$ for $1\le i\le n$ and $E_{ij}+E_{ji}$ for $i<j$, so

$$
\dim S=n+\binom n2=\frac{n(n+1)}2.
$$

The [dimension formula for a sum of subspaces](../../../../../../../dimension-formula-for-a-sum-of-subspaces.md) now gives

$$
\begin{aligned}
\dim(V\cap S)
&=\dim V+\dim S-\dim(V+S)\\
&\ge\dim V+\frac{n(n+1)}2-n^2\\
&=\dim V-\binom n2>0.
\end{aligned}
$$

Choose $0\ne A\in V\cap S$. It belongs to $V$ and is a [symmetric matrix](../../../../../../../symmetric-matrix.md), so part (a)(i) makes it a [diagonalisable matrix](../../../../../../../diagonalizable-matrix.md). The preceding example shows that the strict threshold is sharp.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [b](../../b.md)
3. [4](../../../4.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
