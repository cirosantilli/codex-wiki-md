<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under a proper [rotation matrix](../../../../../rotation-matrix.md) $R$, the product of coordinates transforms as a rank-$n$ [tensor](../../../../../tensor.md). The unit ball is unchanged by the substitution $\mathbf y=R\mathbf x$, whose [Jacobian determinant](../../../../../jacobian-determinant.md) is one. Hence

$$
\begin{aligned}
R_{i_1j_1}\cdots R_{i_nj_n}S_{j_1\cdots j_n}
&=\int_B(R\mathbf x)_{i_1}\cdots(R\mathbf x)_{i_n}\,dV_{\mathbf x}\\
&=\int_B y_{i_1}\cdots y_{i_n}\,dV_{\mathbf y}=S_{i_1\cdots i_n}.
\end{aligned}
$$

Thus $S$ is an [isotropic tensor](../../../../../isotropic-tensor.md). An [isotropic second-rank tensor](../../../../../isotropic-second-rank-tensor.md) has the form $S_{ij}=A\delta_{ij}$. Taking the [trace](../../../../../matrix-trace.md) and using [spherical coordinates](../../../../../spherical-coordinate-system.md),

$$
3A=\int_B|\mathbf x|^2\,dV=4\pi\int_0^1r^4\,dr=\frac{4\pi}5.
$$

Therefore the [isotropic second moment of a ball](../../../../../isotropic-second-moment-of-a-ball.md) is

$$
\boxed{S_{ij}=\frac{4\pi}{15}\delta_{ij}.}
$$

An [isotropic third-rank tensor](../../../../../isotropic-third-rank-tensor.md) has the form $B\epsilon_{ijk}$, but $S_{ijk}$ is symmetric in every pair of indices, forcing $B=0$. Alternatively, $\mathbf x\mapsto-\mathbf x$ makes its integrand odd on the ball. Thus

$$
\boxed{S_{ijk}=0.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
