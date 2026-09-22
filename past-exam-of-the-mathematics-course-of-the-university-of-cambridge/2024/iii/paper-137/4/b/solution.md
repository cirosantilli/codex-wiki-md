<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\tau=x+iy$ and $\sigma=\operatorname{Re}s>1$. The positive-definite quadratic form

$$
Q_\tau(m,n)=|m\tau+n|^2
$$

is bounded below by $C_\tau(m^2+n^2)$ for some $C_\tau>0$. Hence

$$
\sum_{(m,n)\ne(0,0)}
\left|\frac{y^s}{|m\tau+n|^{2s}}\right|
\leq y^\sigma C_\tau^{-\sigma}
\sum_{(m,n)\ne(0,0)}(m^2+n^2)^{-\sigma},
$$

and the last two-dimensional [lattice sum](../../../../../../lattice-sum.md) converges for $\sigma>1$. Thus the [nonholomorphic Eisenstein series](../../../../../../nonholomorphic-eisenstein-series.md) converges absolutely.

For $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma(1)$,

$$
\operatorname{Im}(\gamma\tau)=\frac{y}{|c\tau+d|^2}
$$

and

$$
m\gamma\tau+n
=\frac{(ma+nc)\tau+(mb+nd)}{c\tau+d}.
$$

The map $(m,n)\mapsto(ma+nc,mb+nd)$ permutes $\mathbb Z^2\setminus\{0\}$, so absolute convergence permits reindexing and gives $G(\gamma\tau,s)=G(\tau,s)$. Hence $G(\tau,s)\in W_0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
