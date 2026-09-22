<h1 id="40a/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [exact line search for a positive-definite quadratic](../../../../../../../exact-line-search-for-a-positive-definite-quadratic.md) gives

$$
f(x_{k+1})-f(x_k)
=-\frac12\frac{(r_k^Tr_k)^2}{r_k^TAr_k}.
$$

Using

$$
f(x_k)-f(x^*)=\frac12r_k^TA^{-1}r_k
$$

produces the stated ratio formula. If $l$ and $L$ are the extreme [eigenvalues](../../../../../../../eigenvalue.md),

$$
r_k^TAr_k\leq Lr_k^Tr_k,
\qquad
r_k^TA^{-1}r_k\leq l^{-1}r_k^Tr_k.
$$

Hence the fraction in the ratio is at least $l/L$, and iteration yields

$$
f(x_k)-f(x^*)\leq(1-l/L)^k\{f(x_0)-f(x^*)\}.
$$

When $n=1$, $l=L$, so the right side is zero after one iteration: exact line search reaches the solution in a single step.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [40A](../../../40a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
