<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On a grid $G\subset[-L,L]$ with mesh proportional to $\varepsilon$, [Hoeffding inequality](../../../../../../hoeffding-inequality.md) and a union bound give

$$
\mathbb P\left(\max_{x,y\in G}|k(x,y)-\phi(x)^T\phi(y)|>\varepsilon/2\right)
\leq C\frac{L^2}{\varepsilon^2}e^{-c\ell\varepsilon^2}.
$$

The density of $W$ has exponential tails. A [Chernoff bound](../../../../../../chernoff-bound.md) therefore shows that $\ell^{-1}\sum_i|W_i|$ is bounded by an absolute constant except on an event of probability $e^{-c'\ell}$. On that event, both the empirical kernel and $k$ are uniformly Lipschitz, so every pair $(x,y)$ is approximated by its nearest grid pair with total error at most $\varepsilon/2$. Enlarging constants and using $0<\varepsilon\leq1$ yields

$$
\boxed{\mathbb P\left(\sup_{x,y\in[-L,L]}|k(x,y)-\phi(x)^T\phi(y)|\geq\varepsilon\right)
\leq\frac{C_1L^2}{\varepsilon^2}e^{-C_2\ell\varepsilon^2}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
