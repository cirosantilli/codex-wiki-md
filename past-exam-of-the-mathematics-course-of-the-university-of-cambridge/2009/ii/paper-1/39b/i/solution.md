<h1 id="39b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the diagonal entries of $A$ are nonzero. The [Relaxed Jacobi method](../../../../../../weighted-jacobi-method.md) simultaneously updates every component using the preceding iterate:

$$
x_i^{(\nu+1)}=(1-\omega)x_i^{(\nu)}+\frac{\omega}{a_{ii}}
\left(b_i-\sum_{j\ne i}a_{ij}x_j^{(\nu)}\right).
$$

In matrix form, with $D=\operatorname{diag}(A)$, this is $x^{(\nu+1)}=x^{(\nu)}+\omega D^{-1}(b-Ax^{(\nu)})$. The ordinary [Jacobi method](../../../../../../jacobi-method.md) has $\omega=1$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [39B](../../39b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
