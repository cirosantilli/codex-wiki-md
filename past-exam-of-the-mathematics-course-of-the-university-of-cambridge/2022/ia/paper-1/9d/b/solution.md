<h1 id="9d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First suppose $x_n\to L>0$. Continuity of the [natural logarithm](../../../../../../natural-logarithm.md) gives $\log x_n\to\log L$. Part (a), applied to this sequence, yields

$$
\frac1n\sum_{k=1}^n\log x_k\longrightarrow\log L.
$$

Applying the continuous [exponential function](../../../../../../exponential-function.md),

$$
\sqrt[n]{x_1x_2\cdots x_n}
=\exp\!\left(\frac1n\sum_{k=1}^n\log x_k\right)
\longrightarrow L.
$$

If $L=0$, then for every $\varepsilon>0$ all sufficiently late $x_k$ are below $\varepsilon$. Splitting off the fixed initial product shows that the limsup of the geometric means is at most $\varepsilon$; hence it is zero. This proves the [geometric mean of a sequence](../../../../../../geometric-mean-of-a-sequence.md) result in all cases.

Now suppose

$$
r_n=\frac{x_n}{x_{n-1}}\longrightarrow r.
$$

The telescoping product is

$$
x_n=x_0\prod_{k=1}^nr_k.
$$

Therefore

$$
\sqrt[n]{x_n}
=x_0^{1/n}\sqrt[n]{r_1r_2\cdots r_n}
\longrightarrow 1\cdot r,
$$

and so

$$
\boxed{\lim_{n\to\infty}\sqrt[n]{x_n}
=\lim_{n\to\infty}\frac{x_n}{x_{n-1}}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
