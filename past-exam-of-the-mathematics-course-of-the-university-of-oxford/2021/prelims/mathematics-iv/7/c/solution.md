<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

For [multivariable Newton iteration](../../../../../../multivariable-newton-iteration.md), use the [Jacobian matrix](../../../../../../jacobian-matrix.md)

$$
D\mathbf f(x,y,z)=\begin{pmatrix}
y&x&-3\\
2x&2y&2z\\
\cos x&e^y&-4
\end{pmatrix}.
$$

At $\mathbf x_0=(1/2,-1/2,1/2)$, direct evaluation gives

$$
\mathbf f(\mathbf x_0)=\begin{pmatrix}-3/4\\-1/4\\\sin(1/2)+e^{-1/2}-2\end{pmatrix}.
$$

With $\mathbf s_0=\mathbf x_1-\mathbf x_0$, the required [linear system](../../../../../../system-of-linear-equations.md) is therefore

$$
\boxed{\begin{pmatrix}
-1/2&1/2&-3\\
1&-1&1\\
\cos(1/2)&e^{-1/2}&-4
\end{pmatrix}\begin{pmatrix}s_x\\s_y\\s_z\end{pmatrix}
=\begin{pmatrix}3/4\\1/4\\2-\sin(1/2)-e^{-1/2}\end{pmatrix}.}
$$

After solving this [linear system](../../../../../../system-of-linear-equations.md), form $\boxed{\mathbf x_1=\mathbf x_0+\mathbf s_0}$. To get the second iterate, evaluate both the [Jacobian matrix](../../../../../../jacobian-matrix.md) and the residual anew at $\mathbf x_1$, solve

$$
D\mathbf f(\mathbf x_1)\mathbf s_1=-\mathbf f(\mathbf x_1),
$$

and set $\boxed{\mathbf x_2=\mathbf x_1+\mathbf s_1}$. Reusing the initial [Jacobian matrix](../../../../../../jacobian-matrix.md) would define a different iteration. The requested [linear system](../../../../../../system-of-linear-equations.md) has deliberately been left unsolved.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [7](../../7.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
