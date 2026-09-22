<h1 id="22i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $P_N$ be the orthogonal projection of $\ell^2$ onto the span of its first $N$ standard basis vectors. Then $P_Ny\to y$ for every $y\in\ell^2$, and $\lVert I-P_N\rVert\leq1$.

Let $T$ be compact and let

$$
K=\overline{T(B)},
$$

where $B$ is the closed unit ball. The set $K$ is compact. Given $\varepsilon>0$, choose a finite $\varepsilon/3$-net $y_1,\ldots,y_m$ in $K$. Pointwise convergence lets us choose $N$ such that

$$
\lVert(I-P_N)y_j\rVert<\frac{\varepsilon}{3}
$$

for every $j$. If $y\in K$ and $\lVert y-y_j\rVert<\varepsilon/3$, then

$$
\lVert(I-P_N)y\rVert
\leq\lVert(I-P_N)(y-y_j)\rVert
+\lVert(I-P_N)y_j\rVert
<\frac{2\varepsilon}{3}.
$$

Thus $P_N\to I$ uniformly on $K$, and

$$
\lVert P_NT-T\rVert
=\sup_{\lVert x\rVert\leq1}\lVert(P_N-I)Tx\rVert
\longrightarrow0.
$$

Each $P_NT$ has image in an $N$-dimensional space, so it has finite rank. This [coordinate-projection approximation of a compact operator](../../../../../../coordinate-projection-approximation-of-a-compact-operator.md) proves the result.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22I](../../22i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
