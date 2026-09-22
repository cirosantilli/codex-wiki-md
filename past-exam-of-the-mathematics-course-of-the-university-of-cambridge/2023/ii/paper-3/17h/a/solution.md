<h1 id="17h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We prove the [Quadratic Turan edge bound](../../../../../../quadratic-turan-edge-bound.md) by induction. The case $r=1$ is immediate. For $r\geq2$, if $G$ contains no $K_r$, the induction hypothesis for $r-1$ gives the stronger bound. Otherwise choose a copy $S$ of $K_r$. Every vertex outside $S$ has at most $r-1$ neighbours in $S$, since one adjacent to all of $S$ would complete a $K_{r+1}$. Thus the number of edges having at least one endpoint in $S$ is at most

$$
\binom r2+(n-r)(r-1)
=(r-1)\left(n-\frac r2\right).
$$

The graph $G-S$ is still $K_{r+1}$-free, so induction on the number of vertices gives

$$
\begin{aligned}
e(G)
&\leq
\left(1-\frac1r\right)\frac{(n-r)^2}{2}
+(r-1)\left(n-\frac r2\right)\\
&=\boxed{\left(1-\frac1r\right)\frac{n^2}{2}}.
\end{aligned}
$$

This proves the stated form of [Turan theorem](../../../../../../turan-s-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17H](../../17h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
