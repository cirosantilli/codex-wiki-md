<h1 id="29j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $h=n^{-1/3}$. Away from the boundary, the estimator is

$$
\widehat f_n(x)=\frac1{nh}\sum_{i=1}^n
\mathbf1_{\{|X_i-x|\leq h/2\}}.
$$

Its variance is at most

$$
\frac1{nh^2}\mathbb P(|X_1-x|\leq h/2)
\leq\frac1{nh}=n^{-2/3},
$$

and the [bias of a kernel density estimator](../../../../../../bias-of-a-kernel-density-estimator.md) is bounded by $h\|f'\|_\infty/2$, so its squared bias is at most $h^2/4$. This gives the claimed bound, with room to spare, whenever the full window lies in the support.

At $x=0$, however, the assertion is false as printed. For example

$$
f(x)=\frac12e^{-x/2},\qquad x\geq0,
$$

satisfies $\sup(|f|+|f'|)=3/4<1$, but

$$
\mathbb E\widehat f_n(0)longrightarrow\frac{f(0)}2=\frac14,
$$

whereas $f(0)=1/2$. The mean-square error therefore tends to $1/16$, contradicting a bound tending to zero. The intended statement needs $x\geq h/2$, a boundary correction, or a condition such as $f(0)=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29J](../../29j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
