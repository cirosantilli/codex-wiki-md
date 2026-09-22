<h1 id="13a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because the parameter enters through $\lambda wy$,

$$
L(y;\lambda_0)
=L(y;\lambda)-(\lambda-\lambda_0)wy
=y^{m+1}-\varepsilon^m\mu wy.
$$

Use this as $f$ in part (a). The necessary orthogonality condition is

$$
0=\int_0^1y_0\left(y^{m+1}-\varepsilon^m\mu wy\right)dx.
$$

With $y=\varepsilon y_0+\varepsilon^2y_1$ and $\mu=O(1)$,

$$
y^{m+1}=\varepsilon^{m+1}y_0^{m+1}+O(\varepsilon^{m+2}),
\qquad
wy=\varepsilon wy_0+O(\varepsilon^2).
$$

Consequently

$$
0=\varepsilon^{m+1}
\left[
\int_0^1y_0^{m+2}\,dx
-\mu\int_0^1wy_0^2\,dx
\right]
+O(\varepsilon^{m+2}).
$$

The normalization makes the second [integral](../../../../../../integral.md) one. Divide by $\varepsilon^{m+1}$ to obtain

$$
\boxed{\mu=\int_0^1y_0^{m+2}\,dx+O(\varepsilon)}.
$$

This is the [leading nonlinear eigenvalue shift in a Sturm-Liouville problem](../../../../../../leading-nonlinear-eigenvalue-shift-in-a-sturm-liouville-problem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13A](../../13a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
