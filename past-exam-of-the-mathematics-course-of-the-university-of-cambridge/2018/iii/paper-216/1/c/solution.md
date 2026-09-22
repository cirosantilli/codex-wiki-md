<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $A_n=\sum_{i=1}^{m_n}f(X_i)$ and $T_n=\sum_{i=m_n+1}^n f(X_i)$. Since $|A_n|\leq Bm_n$, $\operatorname{Var}(A_n)\leq B^2m_n^2$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) applied to the centered sums gives

$$
\sqrt{\operatorname{Var}(A_n+T_n)}
\leq\sqrt{\operatorname{Var}(A_n)}+\sqrt{\operatorname{Var}(T_n)}.
$$

Divide by $\sqrt n$. The first term is at most $Bm_n/\sqrt n\to0$, while part (b) and $(n-m_n)/n\to1$ give a limsup of at most $\sqrt{\gamma\operatorname{Var}_\mu(f)}$ for the second. Squaring proves

$$
\boxed{\limsup_{n\to\infty}\frac1n\operatorname{Var}\!\left(\sum_{i=1}^n f(X_i)\right)\leq\gamma\operatorname{Var}(f(Y)).}
$$

This argument also covers $\operatorname{Var}_\mu(f)=0$; it does not require independence between the discarded prefix and the retained path. The same chain-dependent $\gamma$ as in part (b) suffices.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
