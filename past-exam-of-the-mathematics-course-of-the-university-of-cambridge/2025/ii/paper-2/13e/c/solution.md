<h1 id="13e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set

$$
u=\frac{1-z}{2}.
$$

This Möbius change sends $z=1,-1,\infty$ to $u=0,1,\infty$, respectively, without changing the corresponding exponents. The hypergeometric P-symbol has exponents

$$
\begin{array}{c|ccc}
&0&1&\infty\\ \hline
&0&0&A\\
&1-C&C-A-B&B.
\end{array}
$$

Matching it with $(0,1/2)$ at both finite singularities and $(-n,n)$ at infinity gives

$$
C=\frac12,\qquad A=n,\qquad B=-n.
$$

The exponent-zero solution normalized to one at $u=0$ is therefore

$$
\boxed{w_1(z)=F\left(n,-n;\frac12;\frac{1-z}{2}\right).}
$$

The second standard local solution at $u=0$ is

$$
u^{1-C}F(A-C+1,B-C+1;2-C;u).
$$

After absorbing the constant $2^{-1/2}$ into its normalization, this becomes

$$
\boxed{
w_2(z)=(1-z)^{1/2}
F\left(-n+\frac12,n+\frac12;\frac32;\frac{1-z}{2}\right).}
$$

Their exponents at $z=1$ are $0$ and $1/2$, so they are linearly independent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13E](../../13e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
