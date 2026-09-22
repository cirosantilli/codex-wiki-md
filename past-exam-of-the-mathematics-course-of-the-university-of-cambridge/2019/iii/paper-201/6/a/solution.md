<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The count $N_t=M(0,t]$ is a rate-$\lambda$ [Poisson process](../../../../../../poisson-process.md). Over a time interval $(s,t]$, the increment

$$
X_t-X_s=\sum_{n=N_s+1}^{N_t}g(Y_n)
$$

depends only on the Poisson points and marks in that interval. Disjoint intervals give independent increments, and the distribution depends only on $t-s$. The paths are càdlàg step functions, $X_0=0$, and

$$
\mathbb P(X_{t+h}\ne X_t)\leq\mathbb P(N_{t+h}-N_t\geq1)
=1-e^{-\lambda h}\longrightarrow0.
$$

Thus $X$ is stochastically continuous and

$$
\boxed{(X_t)_{t\geq0}\text{ is a compound Poisson process, hence a Lévy process}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
