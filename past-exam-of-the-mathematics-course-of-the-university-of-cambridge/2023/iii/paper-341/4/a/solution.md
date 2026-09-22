<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the real $L^2$ [inner product](../../../../../../inner-product.md) of the equation with $u$. The homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) and [integration by parts](../../../../../../integration-by-parts.md) give

$$
\begin{aligned}
\frac12\frac d{dt}\|u(t)\|_{L^2}^2
&=\int_{-1}^1u u_{xx}\,dx+\alpha\int_{-1}^1u u_x\,dx\\
&=-\int_{-1}^1|u_x|^2\,dx
+\frac\alpha2[u^2]_{-1}^{1}\\
&=-\|u_x\|_{L^2}^2\leq0.
\end{aligned}
$$

Thus $\|u(t)\|_{L^2}\leq\|u_0\|_{L^2}$, and applying the same estimate to the difference of two solutions gives continuous dependence on the initial data. The constant-advection term is [skew-symmetric](../../../../../../skew-symmetric-matrix.md) under these boundary conditions and contributes no energy. Hence

$$
\boxed{\text{the problem is well posed in }L^2\text{ for every }\alpha\in\mathbb R.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
