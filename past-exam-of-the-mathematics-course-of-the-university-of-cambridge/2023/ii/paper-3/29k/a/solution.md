<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For every finite collection of positive times, $(B_{t_1},\ldots,B_{t_m})$ is a linear transformation of the corresponding values of $W$, so $B$ is a centered [Gaussian process](../../../../../../gaussian-process.md). If $0<s\leq t$, then

$$
\mathbb E[B_sB_t]
=st\,\mathbb E[W_{1/s}W_{1/t}]
=st\min\!\left(\frac1s,\frac1t\right)
=s
=\min(s,t).
$$

Thus $B$ has the covariance of [Brownian motion](../../../../../../brownian-motion-split.md).

Its paths are continuous for $t>0$. As $t\downarrow0$, put $u=1/t$. The given almost-sure limit gives

$$
B_t=tW_{1/t}=\frac{W_u}{u}\longrightarrow0=B_0.
$$

The [Gaussian-process characterization of Brownian motion](../../../../../../gaussian-process-characterization-of-brownian-motion.md) now proves the [time inversion of Brownian motion](../../../../../../time-inversion-of-brownian-motion.md):

$$
\boxed{(B_t)_{t\geq0}\text{ is a standard Brownian motion}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
