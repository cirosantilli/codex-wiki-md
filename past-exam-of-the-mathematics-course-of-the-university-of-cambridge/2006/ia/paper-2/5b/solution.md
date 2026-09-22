<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

First solve the closed [linear system of differential equations](../../../../../linear-system-of-differential-equations.md) for $x,y$. Its coefficient matrix is $A=\begin{pmatrix}5&3\\2&0\end{pmatrix}$, with [characteristic polynomial](../../../../../characteristic-polynomial.md) $r^2-5r-6=(r-6)(r+1)$. Corresponding [eigenvectors](../../../../../eigenvector.md) are $(3,1)^T$ and $(1,-2)^T$. The homogeneous solution is therefore

$$
\begin{pmatrix}x_h\\y_h\end{pmatrix}
=C_1e^{6t}\begin{pmatrix}3\\1\end{pmatrix}
+C_2e^{-t}\begin{pmatrix}1\\-2\end{pmatrix}.
$$

Use separate exponential particular solutions for the two forcing frequencies. Solving $(2I-A)u=(1,0)^T$ and $(I-A)v=(0,2)^T$ gives $u=(-1/6,-1/6)^T$ and $v=(-3/5,4/5)^T$. Hence

$$
\boxed{x=3C_1e^{6t}+C_2e^{-t}-\frac16e^{2t}-\frac35e^t,\qquad
y=C_1e^{6t}-2C_2e^{-t}-\frac16e^{2t}+\frac45e^t.}
$$

The third equation then gives $z'=4C_1e^{6t}-C_2e^{-t}-e^{2t}/3+6e^t/5$. Integrating,

$$
\boxed{z=\frac23C_1e^{6t}+C_2e^{-t}-\frac16e^{2t}+\frac65e^t+C_3.}
$$

The three arbitrary constants span the general solution: two arise from the first-order $x,y$ subsystem and one from integrating $z$.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
