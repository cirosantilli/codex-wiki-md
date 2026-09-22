<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Suppose for contradiction that the [critical probability for site percolation on the triangular lattice](../../../../../../critical-probability-for-site-percolation-on-the-triangular-lattice.md) satisfied $p_c>1/2$. Then $p=1/2$ would be subcritical, so [exponential decay of subcritical percolation](../../../../../../exponential-decay-of-subcritical-percolation.md) would give constants $C,c>0$ such that the probability that a fixed site has an open path to distance $N$ is at most $Ce^{-cN}$.

Every left-to-right open crossing of an $N$ by $N$ rhombus contains a site on its left side joined to distance at least $N$. There are $O(N)$ possible starting sites, so the [union bound](../../../../../../boole-s-inequality.md) would imply

$$
\mathbb P_{1/2}(\text{left-to-right crossing})
\leq C'Ne^{-cN}\longrightarrow0.
$$

Planar self-duality and symmetry instead make this crossing probability exactly $1/2$ at every $N$. This contradiction proves $p_c\leq1/2$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
