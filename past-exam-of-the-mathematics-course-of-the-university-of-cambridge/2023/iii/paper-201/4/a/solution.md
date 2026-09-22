<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $0\leq s\leq t$, write $B_t=B_s+(B_t-B_s)$. The increment is independent of $\mathcal F_s$ and is normally distributed with variance $t-s$. Its moment generating function gives

$$
\begin{aligned}
\mathbb E[M_\lambda(t)\mid\mathcal F_s]
&=e^{\lambda B_s-\lambda^2s/2}
\mathbb E\left[e^{\lambda(B_t-B_s)-\lambda^2(t-s)/2}\right]\\
&=M_\lambda(s).
\end{aligned}
$$

The process is integrable for every real $\lambda$, so it is the [exponential Brownian martingale](../../../../../../exponential-brownian-martingale.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
