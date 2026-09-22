<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

A [principal body frame](../../../../../principal-body-frame.md) is an orthonormal basis $\mathbf e_a(t)$ fixed in the rotating body and aligned with its principal axes. If $R(t)$ is the rotation matrix whose columns are these vectors, differentiating $R^TR=I$ shows that $\dot R R^T$ is [skew-symmetric](../../../../../skew-symmetric-matrix.md). Every skew-symmetric linear map in three dimensions is cross product with a unique vector $\boldsymbol\omega$, so

$$
\boxed{\dot{\mathbf e}_a=\boldsymbol\omega\mathbin\times\mathbf e_a.}
$$

For any vector $\mathbf A=A_a\mathbf e_a$,

$$
\left(\frac{d\mathbf A}{dt}\right)_{
m space}
=\dot A_a\mathbf e_a+\boldsymbol\omega\mathbin\times\mathbf A.
$$

Applying this to the conserved angular momentum

$$
\mathbf L=I_1\omega_1\mathbf e_1+I_2\omega_2\mathbf e_2+I_3\omega_3\mathbf e_3
$$

gives the [Euler equations for a torque-free rigid body](../../../../../euler-equations-for-a-torque-free-rigid-body.md):

$$
\boxed{
I_1\dot\omega_1=(I_2-I_3)\omega_2\omega_3,
\quad
I_2\dot\omega_2=(I_3-I_1)\omega_3\omega_1,
\quad
I_3\dot\omega_3=(I_1-I_2)\omega_1\omega_2.}
$$

Multiplying these equations respectively by $\omega_i$ and summing proves conservation of [kinetic energy](../../../../../kinetic-energy.md); multiplying by $I_i\omega_i$ and summing proves conservation of squared [angular momentum](../../../../../angular-momentum.md). Thus the [torque-free rigid-body invariants](../../../../../torque-free-rigid-body-invariants.md) are

$$
2E=I_1\omega_1^2+I_2\omega_2^2+I_3\omega_3^2,
\qquad
L^2=I_1^2\omega_1^2+I_2^2\omega_2^2+I_3^2\omega_3^2.
$$

Solving these two linear equations for the first two squared components gives

$$
\omega_1^2=
\frac{L^2-2EI_2+I_3(I_2-I_3)\omega_3^2}{I_1(I_1-I_2)},
$$



$$
\omega_2^2=
\frac{L^2-2EI_1+I_3(I_1-I_3)\omega_3^2}{I_2(I_2-I_1)}.
$$

Using $I_3\dot\omega_3=(I_1-I_2)\omega_1\omega_2$ yields the [quartic equation for one component of torque-free angular velocity](../../../../../quartic-equation-for-one-component-of-torque-free-angular-velocity.md):

$$
\boxed{
\dot\omega_3^2=f(\omega_3)
=-\frac{
\left[L^2-2EI_2+I_3(I_2-I_3)\omega_3^2\right]
\left[L^2-2EI_1+I_3(I_1-I_3)\omega_3^2\right]
}{I_1I_2I_3^2}.}
$$

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
