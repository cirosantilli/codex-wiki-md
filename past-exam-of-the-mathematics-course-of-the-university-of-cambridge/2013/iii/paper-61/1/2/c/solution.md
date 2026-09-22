<h1 id="1/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any degree-at-most-$n$ [trigonometric polynomial](../../../../../../../trigonometric-polynomial.md) $t_n$, linearity and reproduction give

$$
f-v_{n,m}(f)
=(f-t_n)-v_{n,m}(f-t_n).
$$

The [operator norm](../../../../../../../operator-norm.md) bound in the preceding part yields

$$
\|f-v_{n,m}(f)\|_\infty
\le\left(2+\frac{2n}{m}\right)\|f-t_n\|_\infty
\le2(M+1)\|f-t_n\|_\infty.
$$

Take the infimum over all such [trigonometric polynomials](../../../../../../../trigonometric-polynomial.md). By the definition of [best uniform approximation](../../../../../../../best-uniform-approximation.md),

$$
\boxed{\|f-v_{n,m}(f)\|_\infty\le2(M+1)E_n(f)}.
$$

No choice of a minimizer is needed for this argument. It is an instance of the [polynomial reproduction error bound](../../../../../../../polynomial-reproduction-error-bound.md): a bounded linear reproducing operator has error at most $1+\|P\|$ times the optimal error.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [Paper 61](../../../../paper-61-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
