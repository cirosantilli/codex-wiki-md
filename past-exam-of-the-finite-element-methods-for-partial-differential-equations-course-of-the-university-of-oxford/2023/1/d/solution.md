<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $x_1,\ldots,x_N$ be the interior nodes, and let $\phi_1,\ldots,\phi_N$ be the nodal [basis](../../../../basis.md) of the common [conforming finite element space](../../../../conforming-finite-element-space.md), with $\phi_j(x_i)=\delta_{ij}$ and zero boundary values. These [piecewise-linear hat functions](../../../../piecewise-linear-hat-function.md) give the expansions

$$
u_h=\sum_{j=1}^N U_j\phi_j,\qquad w_h=\sum_{j=1}^N W_j\phi_j.
$$

Testing the first equation with $\phi_i$ and then the second equation with $\phi_i$ gives the [linear system](../../../../system-of-linear-equations.md)

$$
\boxed{\begin{pmatrix}S&-M\\M&S\end{pmatrix}\begin{pmatrix}U\\W\end{pmatrix}=\begin{pmatrix}0\\F\end{pmatrix},\qquad
S_{ij}=\int_\Omega\nabla\phi_j\cdot\nabla\phi_i,\quad
M_{ij}=\int_\Omega\phi_j\phi_i,\quad
F_i=\int_\Omega f\phi_i.}
$$

Here $S$ is the diffusion [stiffness matrix](../../../../stiffness-matrix.md) and $M$ the [mass matrix](../../../../mass-matrix.md). Their entries are symmetric in $i,j$, so both are [symmetric matrices](../../../../symmetric-matrix.md).

For $c\in\mathbb R^N$, put $v_c=\sum_jc_j\phi_j$. The two [quadratic forms](../../../../quadratic-form-split.md) are

$$
c^{\mathsf T}Mc=\|v_c\|_0^2,\qquad c^{\mathsf T}Sc=\|\nabla v_c\|_0^2.
$$

If $c\ne0$, the [linear independence](../../../../linear-independence.md) of the [basis](../../../../basis.md) ensures $v_c\ne0$, so $c^{\mathsf T}Mc>0$. If $c^{\mathsf T}Sc=0$, the [Poincaré inequality](../../../../poincare-inequality.md) and zero [Dirichlet boundary condition](../../../../dirichlet-boundary-condition.md) force $v_c=0$, contradicting $c\ne0$. Thus both $S$ and $M$ are [positive-definite matrices](../../../../positive-definite-matrix.md).

For $X=(p,q)\in\mathbb R^N\times\mathbb R^N$, symmetry of $M$ cancels the cross terms:

$$
\begin{aligned}
X^{\mathsf T}AX
&=p^{\mathsf T}Sp-p^{\mathsf T}Mq+q^{\mathsf T}Mp+q^{\mathsf T}Sq\\
&=p^{\mathsf T}Sp+q^{\mathsf T}Sq.
\end{aligned}
$$

Therefore

$$
\boxed{X^{\mathsf T}AX>0\quad(X\ne0),\qquad \frac{A+A^{\mathsf T}}2=\begin{pmatrix}S&0\\0&S\end{pmatrix}.}
$$

This is the positivity of a [quadratic form](../../../../quadratic-form-split.md) intended by the last sentence of the question. For $N>0$, $A$ is a [nonsymmetric matrix](../../../../nonsymmetric-matrix.md), since $M\ne0$. Under the convention that “[positive-definite matrix](../../../../positive-definite-matrix.md)” includes symmetry, that last sentence needs this qualification: the [symmetric part of a matrix](../../../../symmetric-part-of-a-matrix.md) is positive definite. The [quadratic lower bound for a nonsymmetric matrix](../../../../quadratic-lower-bound-for-a-nonsymmetric-matrix.md) still implies that $A$ is an [invertible matrix](../../../../invertible-matrix.md): $AX=0$ would give $X^{\mathsf T}AX=0$, hence $X=0$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../../split.md)
5. [Finite element methods for partial differential equations course of the University of Oxford](../../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
