<h1 id="10b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The symmetric coefficient [matrix](../../../../../../matrix.md) of the [quadratic form](../../../../../../quadratic-form.md) is

$$
Q_a=\begin{pmatrix}a&1/2&1/2\\1/2&0&1/2\\1/2&1/2&0\end{pmatrix},\qquad \det Q_a=\frac{1-a}{4}.
$$

Thus $\boxed{q_a\text{ is nondegenerate if and only if }a\ne1.}$ To obtain its [signature](../../../../../../signature-of-a-quadratic-form.md), put $u=(y+z)/2$ and $v=(y-z)/2$. Completing the square yields

$$
q_a=(u+x)^2-v^2+(a-1)x^2.
$$

The transformation from $(x,y,z)$ to $(u+x,v,x)$ is invertible. The [inertia of a bilinear form](../../../../../../inertia-of-a-bilinear-form.md) is consequently

$$
\boxed{(n_+,n_-)=\begin{cases}(2,1)&a>1,\\(1,2)&a<1.\end{cases}}
$$

If signature means the signed difference $n_+-n_-$, its value is $+1$ for $a>1$ and $-1$ for $a<1$. At $a=1$ the diagonal form has one zero direction, confirming degeneracy.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
