<h1 id="11e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose $\sum_na_n$ diverges. Positivity implies $s_n\to\infty$. Put $t_n=a_n/s_n\in(0,1)$ for $n\geq2$. Since $s_{n-1}=s_n-a_n$,

$$
\frac{s_n}{s_{n-1}}=\frac1{1-t_n}.
$$

If $\sum_nt_n$ converged, then eventually $t_n\leq1/2$ and

$$
\log\frac{s_n}{s_{n-1}}=-\log(1-t_n)\leq2t_n.
$$

Summing would bound the telescoping quantity $\log(s_n/s_1)$, contradicting $s_n\to\infty$. Therefore

$$
\boxed{\sum_{n=1}^\infty\frac{a_n}{s_n}=\infty}.
$$

The converse is true. If $\sum_na_n<\infty$, then $s_n\geq s_1>0$ and

$$
\sum_n\frac{a_n}{s_n}\leq\frac1{s_1}\sum_na_n<\infty.
$$

Taking the contrapositive shows that divergence of the ratio series forces divergence of $\sum_na_n$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
