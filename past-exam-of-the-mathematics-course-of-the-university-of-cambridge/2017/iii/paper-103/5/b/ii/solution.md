<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $\lambda\unlhd\mu$ in the [dominance order on partitions](../../../../../../../dominance-order-on-partitions.md) and $\lambda\ne\mu$. Let $i$ be the first unequal row. Then $\lambda_i<\mu_i$. Put

$$
D_h=\sum_{r=1}^h(\mu_r-\lambda_r).
$$

We have $D_i>0$, and eventually $D_h=0$. Let $j>i$ be its first return to zero. Then $D_h\geq1$ for $i\leq h<j$ and $\lambda_j>\mu_j$.

Move one box from row $j$ to row $i$. Increasing row $i$ is legal: if $i>1$, then $\lambda_{i-1}=\mu_{i-1}\geq\mu_i>\lambda_i$. Decreasing row $j$ is also legal. If $\lambda_j=\lambda_{j+1}$, then $\mu_{j+1}\leq\mu_j<\lambda_j=\lambda_{j+1}$, forcing $D_{j+1}<0$, a contradiction. Also $\lambda_j>0$. Thus the new list $\nu$ is a [partition of an integer](../../../../../../../partition-of-an-integer.md).

The new deficits equal $D_h-1$ on $i\leq h<j$ and $D_h$ elsewhere, so $\lambda\unlhd\nu\unlhd\mu$. The quantity $\sum_r|\lambda_r-\mu_r|$ decreases by two, since the changed rows were a deficit and a surplus. Repeating must terminate at $\mu$. Hence

$$
\boxed{\lambda\unlhd\mu\quad\Longleftrightarrow\quad\mu\text{ is reachable from }\lambda\text{ by single-box up-moves}.}
$$

The construction proves both termination and preservation of the intermediate dominance inequalities.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
