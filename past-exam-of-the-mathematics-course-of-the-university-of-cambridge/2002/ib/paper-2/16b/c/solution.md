<h1 id="16b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Integrate $F(z)=(1+z^2)^{-(k+1)}$ along the interval $[-R,R]$ closed by the positively oriented upper semicircle, with $R>1$. There is just one enclosed [pole](../../../../../../pole.md), at $i$, of order $k+1$. There,

$$
h(z)=(z-i)^{k+1}F(z)=(z+i)^{-(k+1)}.
$$

Differentiating $k$ times gives

$$
h^{(k)}(z)=(-1)^k\frac{(2k)!}{k!}(z+i)^{-(2k+1)}.
$$

By part (b),

$$
\operatorname{res}(F,i)=\frac{(-1)^k(2k)!}{(k!)^2(2i)^{2k+1}}=\frac{(2k)!}{2^{2k+1}i(k!)^2}.
$$

On the semicircle $|1+z^2|\geq R^2-1$, so its integral has absolute value at most $\pi R/(R^2-1)^{k+1}$, tending to zero. The real integral converges absolutely, so the [residue theorem](../../../../../../residue-theorem.md) and the limit $R\to\infty$ give

$$
\boxed{\int_{-\infty}^{\infty}\frac{dx}{(1+x^2)^{k+1}}=2\pi i\operatorname{res}(F,i)=\pi\frac{(2k)!}{(k!)^2}4^{-k}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16B](../../16b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
