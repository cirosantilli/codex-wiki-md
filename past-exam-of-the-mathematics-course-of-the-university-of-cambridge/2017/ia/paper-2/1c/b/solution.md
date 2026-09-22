<h1 id="1c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $U_0=1$, so the same definition $z_n=x_n/U_{n-1}$ includes $n=1$. Since $U_n=a_nU_{n-1}$ and every $a_n$ is nonzero,

$$
z_{n+1}=\frac{a_nx_n+b_n}{U_n}=z_n+\frac{b_n}{U_n}.
$$

The factor $U_n^{-1}$ is a [discrete integrating factor](../../../../../../discrete-integrating-factor.md) for this [variable-coefficient affine recurrence](../../../../../../variable-coefficient-affine-recurrence.md). Sum the increments as a [telescoping series](../../../../../../telescoping-series.md) and multiply back by $U_n$:

$$
\boxed{z_{n+1}-z_n=\frac{b_n}{U_n},\qquad
x_{n+1}=U_n\left(x_1+\sum_{j=1}^n\frac{b_j}{U_j}\right).}
$$

The identity requires no assumption that the coefficients have the same sign.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1C](../../1c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
