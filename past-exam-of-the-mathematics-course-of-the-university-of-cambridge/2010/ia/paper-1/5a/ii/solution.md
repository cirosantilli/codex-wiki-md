<h1 id="5a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [matrix trace](../../../../../../matrix-trace.md) calculation in (i) gives

$$
\operatorname{tr}(A^TA)=\sum_{i,j}A_{ij}^2\geq0.
$$

A sum of nonnegative real numbers is zero exactly when each is zero. Thus $\boxed{\operatorname{tr}(A^TA)=0\iff A=0}$, so the real [Frobenius inner product](../../../../../../frobenius-inner-product.md) is [positive-definite](../../../../../../positive-definite-bilinear-form.md).

Write $\alpha=\operatorname{tr}(A^TA)$, $\beta=\operatorname{tr}(B^TB)$ and $\gamma=\operatorname{tr}(A^TB)$. If $B\ne0$, then $\beta>0$, and applying the same nonnegativity to $A-tB$ gives

$$
0\leq\operatorname{tr}((A-tB)^T(A-tB))
=\alpha-2t\gamma+t^2\beta.
$$

Taking $t=\gamma/\beta$ yields $\alpha-\gamma^2/\beta\geq0$. If $B=0$, the claimed inequality is immediate. Hence the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) here is

$$
\boxed{\bigl(\operatorname{tr}(A^TB)\bigr)^2
\leq\operatorname{tr}(A^TA)\operatorname{tr}(B^TB).}
$$

When $B\ne0$, equality holds exactly when $\operatorname{tr}((A-(\gamma/\beta)B)^T(A-(\gamma/\beta)B))=0$, hence exactly when $A=(\gamma/\beta)B$. Together with the case $B=0$, the complete equality condition is $\boxed{A,B\text{ are linearly dependent}}$, including the case that either is zero.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5A](../../5a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
