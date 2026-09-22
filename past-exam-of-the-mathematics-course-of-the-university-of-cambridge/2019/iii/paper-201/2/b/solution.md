<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $V=\operatorname{Var}(S_n)=\sum_{m=1}^nv_m$. If $\max_{m\leq n}S_m\geq x$, then

$$
\max_{m\leq n}(S_m+c)^2\geq(x+c)^2.
$$

The [Doob maximal inequality for a nonnegative submartingale](../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) therefore gives

$$
\mathbb P\left(\max_{m\leq n}S_m\geq x\right)
\leq\frac{\mathbb E[(S_n+c)^2]}{(x+c)^2}
=\frac{V+c^2}{(x+c)^2}.
$$

The right side is minimized at $c=V/x$, and substitution gives

$$
\boxed{\mathbb P\left(\max_{1\leq m\leq n}S_m\geq x\right)
\leq\frac{\operatorname{Var}(S_n)}
{\operatorname{Var}(S_n)+x^2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
