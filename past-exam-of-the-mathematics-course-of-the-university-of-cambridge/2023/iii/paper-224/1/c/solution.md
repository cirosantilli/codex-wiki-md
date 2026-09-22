<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $p_k=P_X(k)$. The assumption $p_0=0$ ensures that $X-1$ still takes values in $\{0,1,\ldots\}$, and its [probability mass function](../../../../../../probability-mass-function.md) at $k$ is $p_{k+1}$. Using the paper's unhalved $\ell^1$ convention for the [total variation distance](../../../../../../total-variation-distance.md),

$$
\begin{aligned}
\lVert P_X-P_{X-1}\rVert_{\mathrm{TV}}
&=\sum_{k\geq0}|p_k-p_{k+1}|\\
&=\sum_{k\geq0}\{p_k+p_{k+1}-2\min(p_k,p_{k+1})\}\\
&=1+(1-p_0)-2q=2(1-q).
\end{aligned}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
