<h1 id="41c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At an interior grid point, the five-point [finite difference method](../../../../../../finite-difference-method.md) gives

$$
\nabla^2u(ih,jh,t)
\approx\frac1{h^2}
\left(u_{i+1,j}+u_{i-1,j}+u_{i,j+1}+u_{i,j-1}-4u_{ij}\right).
$$

Let

$$
T=
\begin{pmatrix}
-2&1&&\\
1&-2&\ddots&\\
&\ddots&\ddots&1\\
&&1&-2
\end{pmatrix}\in\mathbb R^{m\times m},
$$

where the zero Dirichlet boundary values are already incorporated. Stack the unknowns with the $y$ index varying fastest. Using the [Kronecker product](../../../../../../kronecker-product.md), define

$$
\boxed{A_x=T\otimes I_m,
\qquad A_y=I_m\otimes T}.
$$

Then the semidiscrete equation is

$$
\boxed{
\frac{d\mathbf u}{dt}
=\frac1{h^2}(A_x+A_y)\mathbf u,
\qquad
\mathbf u(t)\in\mathbb R^{m^2}
}.
$$

Moreover,

$$
A_xA_y
=(T\otimes I)(I\otimes T)
=T\otimes T
=(I\otimes T)(T\otimes I)
=A_yA_x.
$$

**Thus the directional matrices commute, as in the [five-point Dirichlet Laplacian as a Kronecker sum](../../../../../../five-point-dirichlet-laplacian-as-a-kronecker-sum.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [41C](../../41c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
