<h1 id="2h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $K\subseteq K_n$, one of the two directed terms in the given [Hausdorff distance](../../../../../../hausdorff-distance.md) vanishes, and

$$
\rho(K_n,K)=\sup_{x\in K_n}\inf_{y\in K}|x-y|.
$$

Suppose this does not tend to zero. Then some $\varepsilon>0$, a strictly increasing sequence $(n_j)$ and points $x_j\in K_{n_j}$ satisfy

$$
\inf_{y\in K}|x_j-y|\geq\varepsilon.
$$

All $x_j$ lie in the compact set $K_1$, so after passing to a subsequence, $x_j\to x$. For every fixed $m$, eventually $n_j\geq m$, so $x_j\in K_m$ and the closedness of $K_m$ gives $x\in K_m$. Hence $x\in K$, contradicting $|x_j-x|\to0$. Therefore $\rho(K_n,K)\to0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2H](../../2h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
