<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the origin at the [centre of mass](../../../../../center-of-mass.md), so $\int_B\rho\mathbf r\,d^3r=0$, and write $r_i=\mathbf r\cdot\mathbf e_i$ in the specified [orthonormal basis](../../../../../orthonormal-basis.md). The [inertia tensor](../../../../../inertia-tensor.md) is

$$
\boxed{I_{ij}=\int_B\rho(\mathbf r)\left(|\mathbf r|^2\delta_{ij}-r_ir_j\right)\,d^3r.}
$$

Here $\delta_{ij}$ is the [Kronecker delta](../../../../../kronecker-delta.md). For a [rigid body](../../../../../rigid-body-dynamics-split.md) with [angular velocity](../../../../../angular-velocity.md) $\boldsymbol\omega$, this [tensor](../../../../../tensor.md) gives $\mathbf L=\mathbf I\boldsymbol\omega$ and [rotational kinetic energy](../../../../../rotational-kinetic-energy.md) $T=\boldsymbol\omega\cdot\mathbf I\boldsymbol\omega/2$.

The [inertia tensor](../../../../../inertia-tensor.md) is a real [symmetric matrix](../../../../../symmetric-matrix.md), so it admits an [orthonormal basis](../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../eigenvector.md). The lines in these [eigenvector](../../../../../eigenvector.md) directions through the [centre of mass](../../../../../center-of-mass.md) are its [principal axes](../../../../../principal-axis.md); the corresponding [eigenvalues](../../../../../eigenvalue.md) $I_1,I_2,I_3$ are its [principal moments of inertia](../../../../../principal-moment-of-inertia.md):

$$
\boxed{\mathbf I\mathbf e_i=I_i\mathbf e_i,\qquad
\mathbf I=\operatorname{diag}(I_1,I_2,I_3)\quad\text{in principal axes}.}
$$

If an [eigenvalue](../../../../../eigenvalue.md) repeats, the corresponding [principal axes](../../../../../principal-axis.md) need not be unique.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the classical mechanics course of the University of Oxford](../../../../split.md)
6. [Classical mechanics course of the University of Oxford](../../../../../classical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
