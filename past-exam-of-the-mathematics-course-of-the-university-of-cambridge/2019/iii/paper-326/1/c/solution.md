<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md) convention $Ax_j=\sigma_jy_j$ and $A^*y_j=\sigma_jx_j$. Starting from zero gives no component in $\ker A$. Write $x(t)=\sum_jc_j(t)x_j$. The coefficient equations are

$$
c_j'=-\sigma_j^2c_j+\sigma_j\langle f,y_j\rangle,\qquad c_j(0)=0.
$$

Solving these scalar [linear ordinary differential equations](../../../../../../linear-ordinary-differential-equation.md) gives

$$
c_j(t)=\frac{1-e^{-\sigma_j^2t}}{\sigma_j}\langle f,y_j\rangle.
$$

Consequently [asymptotic regularization](../../../../../../asymptotic-regularization.md) has the [spectral regularization method](../../../../../../spectral-regularization-method.md) representation

$$
\boxed{u_\alpha=\sum_j\frac{1-e^{-\sigma_j^2/\alpha}}{\sigma_j}\langle f,y_j\rangle x_j.}
$$

The component of $f$ orthogonal to the closure of the range of $A$ is annihilated by $A^*$ and contributes nothing. The scalar filter satisfies $(1-e^{-\sigma^2/\alpha})/\sigma\leq\min(\sigma/\alpha,1/\sigma)\leq\alpha^{-1/2}$, so every fixed-$\alpha$ reconstruction is a bounded [linear operator](../../../../../../linear-operator.md). Its long-time limit is the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) on admissible data.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
