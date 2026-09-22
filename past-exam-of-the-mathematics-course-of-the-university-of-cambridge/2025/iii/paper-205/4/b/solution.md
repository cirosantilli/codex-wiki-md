<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $R$ be the number of rejections and $I_0$ the true-null indices. For $i\in I_0$, remove $p_i$ and let $R_i$ be the number determined by the corresponding leave-one-out step-up rule. On $\{i\text{ rejected},R=r\}$ one has $p_i\leq\alpha r/m$ and $R_i=r$, while $R_i$ is independent of $p_i$. Hence super-uniformity gives

$$
\mathbb E\frac{\mathbf1_{\{i\text{ rejected}\}}}{R\vee1}
\leq\frac\alpha m.
$$

Summing over $i\in I_0$ proves that the [false discovery rate](../../../../../../false-discovery-rate.md) is at most $|I_0|\alpha/m\leq\alpha$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
