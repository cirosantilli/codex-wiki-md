<h1 id="22h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $X$ have basis $e_1,\ldots,e_d$, and write $x=\sum_ja_je_j$. On the compact coordinate sphere $\sum_j|a_j|=1$, the continuous positive function

$$
(a_1,\ldots,a_d)\longmapsto
\left\lVert\sum_ja_je_j\right\rVert
$$

has a positive minimum $m$. Homogeneity and the [triangle inequality](../../../../../../triangle-inequality.md) therefore give constants $m,M>0$ such that

$$
m\sum_j|a_j|
\leq\left\lVert\sum_ja_je_j\right\rVert
\leq M\sum_j|a_j|.
$$

In particular, each coordinate functional $\phi_j(x)=a_j$ belongs to the [continuous dual space](../../../../../../continuous-dual-space-split.md) $X^*$.

Every member of $X^*$ is norm-continuous, so the [weak topology](../../../../../../weak-topology-split.md) is coarser than the [norm topology](../../../../../../norm-topology.md). Conversely, given $x_0\in X$ and $\varepsilon>0$, the basic weak neighbourhood

$$
U=\left\{x:|\phi_j(x-x_0)|<\frac{\varepsilon}{Md}
\text{ for }1\leq j\leq d\right\}
$$

satisfies $U\subseteq\{x:\lVert x-x_0\rVert<\varepsilon\}$. Thus every norm-open set is weakly open, proving that the two topologies coincide. This is the [finite-dimensional weak and norm topologies coincide](../../../../../../finite-dimensional-weak-and-norm-topologies-coincide.md) theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22H](../../22h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
