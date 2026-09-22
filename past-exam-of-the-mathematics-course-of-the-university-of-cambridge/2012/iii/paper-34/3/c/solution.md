<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $k\geq2$, substitute $r_k=k^{-k}$ and $R=k$ into the exit formula:

$$
\boxed{\mathbb P(S_{r_k}\leq T_k)=\frac{\log k}{\log k+k\log k}=\frac1{k+1}\longrightarrow0.}
$$

Let $\tau_0$ be the first hit of the origin. On any path with $\tau_0<\infty$, continuity makes the radius bounded on $[0,\tau_0]$. For all sufficiently large $k$, that path reaches radius $r_k$ before $\tau_0$ and has not yet reached radius $k$, so it belongs to $\{S_{r_k}\leq T_k\}$. Thus $\{\tau_0<\infty\}$ is contained in the liminf of these events. Fatou's inequality for their indicators gives probability at most $\liminf_k1/(k+1)=0$ for that liminf. Hence the [polar point for planar Brownian motion](../../../../../../polar-point-for-planar-brownian-motion.md) conclusion is

$$
\boxed{\mathbb P(|B_t|>0\text{ for every }t\geq0)=1.}
$$

The argument controls one event for all times, rather than merely proving zero hitting probability at each fixed time.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
