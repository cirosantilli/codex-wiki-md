<h1 id="18/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $S_N$ be the [Fourier partial sum](../../../../../../fourier-partial-sum.md) through frequency $N$. By [orthogonality](../../../../../../orthogonal-vectors.md) and the coefficient formulas,

$$
\int_{-L}^{L}S_N^2\,dx
=\frac{La_0^2}{2}+L\sum_{n=1}^{N}(a_n^2+b_n^2),
\qquad
\int_{-L}^{L}fS_N\,dx=\int_{-L}^{L}S_N^2\,dx.
$$

Expanding the nonnegative squared [L2 norm](../../../../../../l2-norm.md) of the error gives the exact finite identity

$$
\int_{-L}^{L}(f-S_N)^2\,dx
=\int_{-L}^{L}f^2\,dx-\frac{La_0^2}{2}-L\sum_{n=1}^{N}(a_n^2+b_n^2).
$$

For $f$ in the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md), completeness of the [Fourier basis](../../../../../../fourier-basis.md) makes the left-hand side tend to zero. Dividing the resulting equality by $2L$ proves [Parseval's identity](../../../../../../parseval-identity.md):

$$
\boxed{\frac1{2L}\int_{-L}^{L}f(x)^2\,dx
=\frac{a_0^2}{4}+\frac12\sum_{n=1}^\infty(a_n^2+b_n^2)}.
$$

This argument uses [convergence in L2](../../../../../../convergence-in-l2.md) rather than an unqualified exchange of an infinite sum with the [integral](../../../../../../integral-split.md) of its square. The [function](../../../../../../function-split.md) in part (c) is continuous and piecewise polynomial, so these hypotheses hold.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [18](../../../18.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
