<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [piecewise-linear hat functions](../../../../../../piecewise-linear-hat-function.md) have disjoint supports unless their nodes coincide or are neighbours. Direct integration on the two adjacent intervals gives

$$
\int\varphi_i'^2=\frac2h,\quad
\int\varphi_i^2=\frac{2h}3,\quad
\int\varphi_i'\varphi_{i+1}'=-\frac1h,\quad
\int\varphi_i\varphi_{i+1}=\frac h6.
$$

Since $x=x_i+(x-x_i)$ and the hat is symmetric about $x_i=ih$, its load is $F_i=x_i\int\varphi_i=x_i h=ih^2$. Thus the [reaction-diffusion finite element matrix](../../../../../../reaction-diffusion-finite-element-matrix.md) gives the explicit equations

$$
\boxed{\left(\frac2h+\frac{2h}3\right)c_i
+\left(-\frac1h+\frac h6\right)(c_{i-1}+c_{i+1})=ih^2,
\quad 1\leq i\leq M,\quad c_0=c_{M+1}=0.}
$$

The coefficient matrix is a [tridiagonal matrix](../../../../../../tridiagonal-matrix.md) and a [positive-definite matrix](../../../../../../positive-definite-matrix.md) by the energy identity in part (b), hence **nonsingular**. A separate spectral verification uses the sine basis with $\theta_j=j\pi/(M+1)$ and gives

$$
\lambda_j=\frac{2(1-\cos\theta_j)}h
+\frac h3(2+\cos\theta_j)>0.
$$

Both terms are positive for the Dirichlet modes. This also identifies precisely how the diffusion [stiffness matrix](../../../../../../stiffness-matrix.md) and reaction [mass matrix](../../../../../../mass-matrix.md) combine.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
