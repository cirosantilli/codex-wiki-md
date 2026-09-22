<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal F_s=\sigma(W_r:0\leq r\leq s)$. For $0\leq s<t$, the increment $W_t-W_s$ is independent of $\mathcal F_s$ and distributed as $\sqrt{t-s}Z$. Apply part (a) to the translated function $u\mapsto f(W_s+u)$, conditionally on $\mathcal F_s$:

$$
\begin{aligned}
\mathbb E[f(W_t)\mid\mathcal F_s]
&=f(W_s)
+\frac12\int_0^{t-s}
\mathbb E[f''(W_s+\sqrt rZ)\mid\mathcal F_s]\,dr\\
&=f(W_s)
+\frac12\mathbb E\left[
\int_s^t f''(W_r)\,dr\ \middle|\ \mathcal F_s
\right].
\end{aligned}
$$

Therefore

$$
\begin{aligned}
\mathbb E[M_t\mid\mathcal F_s]
&=\mathbb E[f(W_t)\mid\mathcal F_s]
-\frac12\int_0^sf''(W_r)\,dr\\
&\quad-\frac12\mathbb E\left[
\int_s^tf''(W_r)\,dr\ \middle|\ \mathcal F_s
\right]\\
&=f(W_s)-\frac12\int_0^sf''(W_r)\,dr
=M_s.
\end{aligned}
$$

The assumed growth conditions supply integrability, so $(M_t)$ is the [Brownian compensator martingale](../../../../../../brownian-compensator-martingale.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
