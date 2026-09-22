<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On the diagonal,

$$
P^k(x,x)-\pi(x)
=\pi(x)\sum_{i\geq2}\lambda_i^kf_i(x)^2,
$$

so every summand is nonnegative. Let $m=\lceil t_{\mathrm{rel}}\rceil$. For every $i\geq2$,

$$
\lambda_i^{m+1}
\leq\lambda_2^{t_{\mathrm{rel}}}
=\left(1-\frac1{t_{\mathrm{rel}}}\right)^{t_{\mathrm{rel}}}
\leq e^{-1}.
$$

Hence

$$
\frac1{1-\lambda_i}
\leq\frac e{e-1}\frac{1-\lambda_i^{m+1}}{1-\lambda_i}
=\frac e{e-1}\sum_{k=0}^m\lambda_i^k.
$$

Multiply by $\pi(x)f_i(x)^2$ and sum over $i\geq2$ to obtain the required inequality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
