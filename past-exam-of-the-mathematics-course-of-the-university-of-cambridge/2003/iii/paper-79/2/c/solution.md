<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $F$ be any [closed set](../../../../../../closed-set.md). For each $M>0$, choose $K_M$ as above. The probability decomposition

$$
\mathbb P(X_L\in F)\leq\mathbb P(X_L\in F\cap K_M)+\mathbb P(X_L\notin K_M)
$$

reduces the first term to a [compact set](../../../../../../compact-space.md), where the weak upper bound applies. For nonnegative numbers $u_L,v_L$, the inequality $u_L+v_L\leq2\max(u_L,v_L)$ shows that the upper exponential rate of their sum is no larger than the maximum of their upper exponential rates. Hence

$$
\limsup_L\frac1L\log\mathbb P(X_L\in F)
\leq\max\left\{-\inf_{F\cap K_M}I,-M\right\}
\leq\max\left\{-\inf_F I,-M\right\}.
$$

Let $M\to\infty$. This proves the full closed-set upper bound, including when $\inf_F I=+\infty$. The open-set lower bound was already assumed. Combining with part (b), **the weak principle upgrades to a large deviation principle with good rate function $I$**. This is [exponential tightness upgrades a weak large deviation principle](../../../../../../exponential-tightness-upgrades-a-weak-large-deviation-principle.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
