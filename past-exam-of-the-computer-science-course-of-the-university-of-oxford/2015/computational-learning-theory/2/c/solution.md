<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A real [positive-semidefinite kernel](../../../../../positive-semidefinite-kernel-split.md) on an input [set](../../../../../set-split.md) $X$ is a [function](../../../../../function-split.md) $K:X\times X\to\mathbb R$ for which there is an [inner product space](../../../../../inner-product-space.md) $\mathcal F$ and a [feature map](../../../../../feature-map.md) $\phi:X\to\mathcal F$ satisfying

$$
\boxed{K(x,z)=\langle\phi(x),\phi(z)\rangle.}
$$

Equivalently, $K$ is symmetric and every finite [Gram matrix](../../../../../gram-matrix.md) $(K(x_i,x_j))_{i,j}$ is [positive semidefinite](../../../../../positive-semidefinite-matrix.md): $\sum_{i,j}a_ia_jK(x_i,x_j)\geq0$ for all real coefficients $a_i$. An infinite-dimensional [Hilbert space](../../../../../hilbert-space-split.md) is allowed.

Replace every [inner product](../../../../../inner-product-split.md) $x_i\cdot x_j$ in part (b) by $K(x_i,x_j)$ and solve

$$
\boxed{\max_{\alpha\geq0,\ y^T\alpha=0}
\left\{\mathbf1^T\alpha-\frac12\sum_{i,j}\alpha_i\alpha_jy_iy_jK(x_i,x_j)-\frac1{4C}\|\alpha\|^2\right\}.}
$$

This is precisely the [Lagrangian dual problem](../../../../../lagrangian-dual-problem.md) obtained by replacing each original input by $\phi(x_i)$ in the [primal problem](../../../../../primal-problem.md). The weight [vector](../../../../../vector.md) it determines is

$$
w_{\mathcal F}=\sum_i\alpha_i y_i\phi(x_i),
$$

and the intercept follows from the same [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md). For example, if $\alpha_i>0$,

$$
b=y_i\left(1-\frac{\alpha_i}{2C}\right)-\sum_j\alpha_j y_jK(x_j,x_i).
$$

Thus training needs only the finite [Gram matrix](../../../../../gram-matrix.md), even if the [feature map](../../../../../feature-map.md) has infinitely many coordinates. This is the [kernel trick](../../../../../kernel-trick.md). The result is an **[affine linear classifier](../../../../../affine-linear-classifier.md) in the feature space**; its boundary in the original input space can be nonlinear. The squared-slack diagonal term and the equality constraint remain unchanged.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
