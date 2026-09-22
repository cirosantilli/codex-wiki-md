<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a sufficiently large positive $n$ for which $g_n=B_n^{-1}f>0$ throughout the interval. Expanding $B_n(g_n)=f$ gives

$$
f(x)=\sum_{k=0}^n\binom nk g_n(k/n)x^k(1-x)^{n-k}.
$$

Therefore the coefficients

$$
\boxed{c_k=\binom nk g_n(k/n)>0,\qquad 0\le k\le n,}
$$

supply the requested representation, in particular with nonnegative coefficients. This proves [positive Bernstein coefficients for a strictly positive polynomial](../../../../../../positive-bernstein-coefficients-for-a-strictly-positive-polynomial.md). Strict positivity cannot generally be weakened to mere nonnegativity: a nonzero polynomial such as $(x-1/2)^2$ vanishes at an interior point, whereas every basis term is positive there, so no nonnegative-coefficient representation could vanish unless every coefficient were zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
