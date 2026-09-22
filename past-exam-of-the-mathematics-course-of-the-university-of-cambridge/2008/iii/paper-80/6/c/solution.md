<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a=\mu(A)$, $b=\mu(B)$ and $c=\mu(A+B)$. The sum is also symmetric negative definite. Part (a) gives the exponential [norm](../../../../../../norm.md) bounds, while the [triangle inequality](../../../../../../triangle-inequality.md) and submultiplicativity give

$$
\|[e^{xA},B]\|_2\leq\|e^{xA}B\|_2+\|Be^{xA}\|_2
\leq2\|B\|_2e^{xa}.
$$

Applying these estimates to the [exponential product defect identity](../../../../../../exponential-product-defect-identity.md) yields

$$
\|\Phi(t)-e^{t(A+B)}\|_2
\leq2\|B\|_2\int_0^t e^{(t-x)c}e^{x(a+b)}\,dx.
$$

If $c<a+b$, evaluate the scalar integral to obtain the [decaying bound for symmetric negative matrix splitting](../../../../../../decaying-bound-for-symmetric-negative-matrix-splitting.md):

$$
\boxed{\|\Phi(t)-e^{t(A+B)}\|_2
\leq2\|B\|_2\frac{e^{t(a+b)}-e^{tc}}{a+b-c}.}
$$

The sign condition is natural: for every unit vector $v$, $v^T(A+B)v\leq a+b$, so the [Rayleigh quotient](../../../../../../rayleigh-quotient.md) gives $c\leq a+b$.

When $c=a+b$, the integrand equals $e^{tc}$ independently of $x$, giving

$$
\boxed{\|\Phi(t)-e^{t(A+B)}\|_2\leq2t\|B\|_2e^{tc}.}
$$

This also follows by taking the continuous limit of the quotient as $a+b-c\to0$. There is no division-by-zero exception in the original integral argument. All exponents are negative, so these bounds decay for large $t$; they are coarse bounds and need not reproduce the sharper quadratic small-$t$ error.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
