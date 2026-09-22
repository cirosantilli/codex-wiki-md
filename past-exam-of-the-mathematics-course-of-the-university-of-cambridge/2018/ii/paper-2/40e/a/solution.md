<h1 id="40e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With $\mathbf u=(u_1,\ldots,u_n)^T$ and $\mathbf b=h^2(f_1,\ldots,f_n)^T$, the system is

$$
\boxed{
A\mathbf u=\mathbf b,
\qquad
A=
\begin{pmatrix}
-2&1\\
1&-2&1\\
&\ddots&\ddots&\ddots\\
&&1&-2&1\\
&&&1&-2
\end{pmatrix}.}
$$

Its diagonal part is $D=-2I$. The [weighted Jacobi method](../../../../../../weighted-jacobi-method.md), also called the [Relaxed Jacobi method](../../../../../../weighted-jacobi-method.md), is

$$
\mathbf u^{(\nu+1)}
=\mathbf u^{(\nu)}
+\omega D^{-1}
\left(\mathbf b-A\mathbf u^{(\nu)}\right).
$$

Componentwise,

$$
\boxed{
u_i^{(\nu+1)}
=(1-\omega)u_i^{(\nu)}
+\frac{\omega}{2}
\left(u_{i-1}^{(\nu)}+u_{i+1}^{(\nu)}-h^2f_i\right),}
$$

with $u_0^{(\nu)}=u_{n+1}^{(\nu)}=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40E](../../40e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
