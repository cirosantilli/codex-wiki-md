<h1 id="26j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The hypothesis says exactly that $X_n\rightharpoonup0$ in the [Hilbert space](../../../../../../hilbert-space-split.md) $L^2$. We give the constructive [weak Banach–Saks theorem in a Hilbert space](../../../../../../weak-banach-saks-theorem-in-a-hilbert-space.md) argument. Choose $n_1<n_2<\cdots$ inductively so that, for $Y_k=X_{n_k}$,

$$
|\mathbb E(Y_jY_k)|\leq2^{-k}
\qquad(1\leq j<k).
$$

This is possible because each earlier $Y_j$ is an admissible test variable in the weak-convergence assumption. Since $\lVert Y_k\rVert_2\leq1$,

$$
\begin{aligned}
\left\lVert\frac1N\sum_{k=1}^NY_k\right\rVert_2^2
&=\frac1{N^2}\left(
\sum_{k=1}^N\lVert Y_k\rVert_2^2
+2\sum_{1\leq j<k\leq N}\mathbb E(Y_jY_k)
\right)\\
&\leq\frac1N+
\frac2{N^2}\sum_{k=2}^N(k-1)2^{-k}
\longrightarrow0.
\end{aligned}
$$

Therefore

$$
\boxed{\frac1N\sum_{k=1}^NY_k\longrightarrow0
\quad\text{in }L^2.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26J](../../26j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
