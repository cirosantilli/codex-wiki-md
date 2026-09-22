<h1 id="40c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $\nabla F(x^{(k)})=-r^{(k)}$, the [Heavy-ball method](../../../../../../heavy-ball-method.md) is

$$
x^{(k+1)}
=x^{(k)}+\alpha r^{(k)}
+\beta(x^{(k)}-x^{(k-1)}).
$$

Multiplication by $A$ and use of $Ax^{(j)}=b-r^{(j)}$ give the [heavy-ball residual recurrence](../../../../../../heavy-ball-residual-recurrence.md)

$$
\boxed{
r^{(k+1)}
=((1+\beta)I-\alpha A)r^{(k)}
-\beta r^{(k-1)}.}
$$

With the usual initialization $x^{(-1)}=x^{(0)}=0$, both initial residuals equal $b$. Induction in the recurrence shows that

$$
r^{(k)}=p_k(A)b
$$

for a polynomial $p_k$ of degree at most $k$. Therefore

$$
\boxed{
r^{(k)}\in
\operatorname{span}\{b,Ab,\ldots,A^kb\}.}
$$

This is $\mathcal K_k(A,b)$ under the zero-indexed [Krylov subspace](../../../../../../krylov-subspace.md) convention in the question; under the convention whose order-$j$ space ends at $A^{j-1}b$, it is $\mathcal K_{k+1}(A,b)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
