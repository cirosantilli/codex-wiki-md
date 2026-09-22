<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**False.** Let $Z\sim N(0,1)$ and define $X_t=tZ$. This is a centered continuous [Gaussian process](../../../../../../gaussian-process.md). Its [natural filtration](../../../../../../natural-filtration.md) satisfies $Z=X_s/s\in\mathcal F_s^X$ for every $s>0$, and hence, for $0<s<t$,

$$
\mathbb E[X_t\mid\mathcal F_s^X]=tZ=\frac tsX_s\ne X_s
$$

with positive probability. Thus $X$ is not a [martingale](../../../../../../martingale-split.md) and does not belong to the stated martingale class.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
