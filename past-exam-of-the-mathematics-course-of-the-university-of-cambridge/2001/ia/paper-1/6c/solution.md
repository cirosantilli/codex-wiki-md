<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

If $Ax_p=b$, then $Ax=b$ is equivalent to $A(x-x_p)=0$. Thus the solution set is the [affine solution space of a linear equation](../../../../../affine-solution-space-of-a-linear-equation.md) $\boxed{x_p+\ker A}$, and every vector of that form solves the equation.

For the [symmetric matrix](../../../../../symmetric-matrix.md) case, let $Au_i=\lambda_i u_i$. Symmetry gives

$$
\lambda_i(u_i\cdot u_j)=(Au_i)\cdot u_j=u_i\cdot(Au_j)=\lambda_j(u_i\cdot u_j).
$$

Distinct [eigenvalues](../../../../../eigenvalue.md) therefore imply $u_i\cdot u_j=0$. Normalizing the three vectors gives an [orthonormal basis](../../../../../orthonormal-basis.md). Expand $x=\sum_i t_i u_i$ and $b=\sum_i b_i u_i$, with $b_i=b\cdot u_i$. The equation $(A-\lambda_kI)x=b$ becomes $(\lambda_i-\lambda_k)t_i=b_i$ for every $i$. Thus solvability is equivalent to $b_k=0$, and all solutions are

$$
\boxed{x=\sum_{i\ne k}\frac{b\cdot u_i}{\lambda_i-\lambda_k}u_i+\beta u_k,\qquad \beta\in\mathbb R.}
$$

This proves the claimed orthogonality condition and the full solution family rather than only a particular solution.

For the numerical [symmetric matrix](../../../../../symmetric-matrix.md), direct multiplication gives $Au_1=0$ for $u_1=(1,1,1)^T/\sqrt3$, and $Au_2=-\sqrt2\,u_2$ for $u_2=(1,-1,0)^T/\sqrt2$. Their orthogonal complement is spanned by $u_3=(1,1,-2)^T/\sqrt6$, and multiplication gives $Au_3=\sqrt3\,u_3$. The supplied right side has $b\cdot u_1=0$, so the [linear system](../../../../../system-of-linear-equations.md) is solvable. Its other coefficients are $b\cdot u_2=2$ and $b\cdot u_3=3\sqrt2$. Hence

$$
x=-\sqrt2\,u_2+\sqrt6\,u_3+\beta u_1
=(0,2,-2)^T+\frac\beta{\sqrt3}(1,1,1)^T.
$$

Equivalently, **all solutions are**

$$
\boxed{x=(0,2,-2)^T+t(1,1,1)^T,\qquad t\in\mathbb R.}
$$

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
