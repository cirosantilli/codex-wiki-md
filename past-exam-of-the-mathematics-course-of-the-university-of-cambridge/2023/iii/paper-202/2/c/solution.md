<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every simple predictable process is left-continuous and adapted: on $(t_k,t_{k+1}]$ its value is already $\mathcal F_{t_k}$-measurable. Hence any sigma-algebra making all left-continuous adapted processes measurable contains the generators of $\mathcal P$.

Conversely, let $X$ be left-continuous and adapted. For $n\geq1$, define

$$
X_t^{(n)}=X_0\mathbf1_{\{0\}}(t)
+\sum_{k\geq0}X_{k2^{-n}}
\mathbf1_{(k2^{-n},(k+1)2^{-n}]}(t).
$$

On each bounded time interval this is a simple predictable process, and left continuity gives $X_t^{(n)}\to X_t$ for every $t$. Thus $X$ is $\mathcal P$-measurable. This proves that $\mathcal P$ is exactly the smallest sigma-algebra making every left-continuous adapted process measurable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
