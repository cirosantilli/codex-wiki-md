<h1 id="17c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Peano kernel theorem](../../../../../../peano-kernel-theorem.md) says that if a continuous linear functional $L$ annihilates polynomials of degree below $m$, then

$$
L(f)=\int_a^bK(t)f^{(m)}(t)\,dt,
\qquad
K(t)=L\left(\frac{(x-t)_+^{m-1}}{(m-1)!}\right).
$$

Here $m=3$ and

$$
L(f)=f''(0)-f(-1)+2f(0)-f(1).
$$

Applying $L$ to $(x-t)_+^2/2$ gives

$$
K(t)=
\begin{cases}
\frac12(1+t)^2,&-1\leq t<0,\\
-\frac12(1-t)^2,&0\leq t\leq1.
\end{cases}
$$

Hence

$$
|L(f)|
\leq\|f'''\|_\infty\int_{-1}^1|K(t)|\,dt
=\frac13\|f'''\|_\infty.
$$

The smallest candidate is therefore

$$
\boxed{c=\frac13}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17C](../../17c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
