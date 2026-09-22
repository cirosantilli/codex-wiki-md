<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $F(x)=\sum_{n=1}^Nb_ne(n^2x)$. Orthogonality gives

$$
\|F\|_4^4
=\sum_m\left|\sum_{n_1^2+n_2^2=m}b_{n_1}b_{n_2}\right|^2.
$$

The number $r_2(m)$ of representations of $m$ as two squares is at most a constant times its divisor function. Since $m\leq2N^2$, the supplied divisor bound and Cauchy-Schwarz imply

$$
\|F\|_4^4
\lesssim_\epsilon N^\epsilon
\sum_{n_1,n_2}|b_{n_1}|^2|b_{n_2}|^2
=N^\epsilon\|b\|_2^4.
$$

For $2\leq p\leq4$, monotonicity of $L^p$ norms on $[0,1]$ gives $\|F\|_p^p\lesssim_\epsilon N^\epsilon\|b\|_2^p$. For $p\geq4$, use $\|F\|_\infty\leq N^{1/2}\|b\|_2$ to obtain

$$
\|F\|_p^p
\leq\|F\|_\infty^{p-4}\|F\|_4^4
\lesssim_\epsilon N^{p/2-2+\epsilon}\|b\|_2^p.
$$

After enlarging the constant and the harmless epsilon loss, both ranges give

$$
\boxed{C_{p,2}(N)\lesssim_\epsilon N^\epsilon(1+N^{p/2-2}).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 163](../../../paper-163-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
