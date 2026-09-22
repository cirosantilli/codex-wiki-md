<h1 id="21f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Tietze extension theorem](../../../../../../tietze-extension-theorem.md) states: if $X$ is a [normal topological space](../../../../../../normal-space.md), $A\subseteq X$ is closed, and $f:A\to[-M,M]$ is continuous, then there is a continuous $F:X\to[-M,M]$ with $F|_A=f$.

We first prove an approximation lemma. Given continuous $h:A\to[-r,r]$, the closed subsets

$$
A_-=\{x\in A:h(x)\leq-r/3\},
\qquad
A_+=\{x\in A:h(x)\geq r/3\}
$$

are disjoint and closed in $X$. By the [Urysohn lemma](../../../../../../urysohn-s-lemma.md), there is a continuous $g:X\to[-r/3,r/3]$ equal to $-r/3$ on $A_-$ and $r/3$ on $A_+$. Then

$$
|h-g|\leq\frac{2r}{3}\quad\hbox{on }A.
$$

Starting with $h_0=f$ and $r_0=M$, apply the lemma recursively to obtain continuous $g_j:X\to\mathbb R$ such that

$$
\|g_j\|_\infty\leq\frac{r_j}{3},
\qquad
h_{j+1}=h_j-g_j|_A,
\qquad
\|h_{j+1}\|_\infty\leq r_{j+1},
$$

where $r_j=M(2/3)^j$. The series

$$
F=\sum_{j=0}^\infty g_j
$$

converges uniformly by the Weierstrass test, so its sum is continuous. On $A$, its remainder after $j$ terms is $h_{j+1}$, which tends uniformly to zero; hence $F|_A=f$. The bounds also keep $F$ in $[-M,M]$ after the standard endpoint-preserving version of the construction, proving the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21F](../../21f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
