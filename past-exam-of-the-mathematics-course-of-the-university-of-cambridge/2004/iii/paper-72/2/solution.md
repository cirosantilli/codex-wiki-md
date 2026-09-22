<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use orthonormal cylindrical bases in the reference and deformed configurations. The radial coordinate remains $\rho$, the angular coordinate becomes $\theta=\Theta+\alpha\xi_3$, and the axial coordinate is unchanged. Removing the rotation of the cylindrical basis, the [deformation gradient](../../../../../deformation-gradient.md) is

$$
A=\begin{pmatrix}1&0&0\\0&1&s\\0&0&1\end{pmatrix},\qquad s=\alpha\rho.
$$

It is a local [simple shear](../../../../../simple-shear.md) with unit [determinant](../../../../../determinant.md). The squared [principal stretches](../../../../../principal-stretch.md) are the [eigenvalues](../../../../../eigenvalue.md) of

$$
A^TA=\begin{pmatrix}1&0&0\\0&1&s\\0&s&1+s^2\end{pmatrix}.
$$

One [principal stretch](../../../../../principal-stretch.md) is one. The remaining squared [principal stretches](../../../../../principal-stretch.md) have product one and sum $2+s^2$. Consequently they can be written $\lambda^2$ and $\lambda^{-2}$, where

$$
\boxed{\lambda=\sqrt{1+s^2/4}+s/2,\qquad\lambda^{-1}=\sqrt{1+s^2/4}-s/2.}
$$

For negative $s$ their ordering reverses, which is immaterial to the [strain energy density](../../../../../strain-energy-density.md) of an isotropic material.

Let the reference length be $L$. By [material isotropy](../../../../../material-isotropy.md), the total [elastic energy](../../../../../elastic-energy.md) and end rotation are

$$
E(\alpha)=2\pi L\int_0^a W(\lambda,\lambda^{-1},1)\rho\,d\rho,\qquad \Theta_{\mathrm{end}}=\alpha L.
$$

For a quasistatic change, [incompressibility](../../../../../incompressible-flow.md) makes the constraint reaction do no work. The velocity on an end section is its rigid rotational velocity; its traction power is the resultant [torque](../../../../../torque.md) times the angular velocity. Thus [conservation of energy](../../../../../conservation-of-energy.md), or equivalently the [torque and axial force of a twisted incompressible cylinder](../../../../../torque-and-axial-force-of-a-twisted-incompressible-cylinder.md) work identity, gives $M\,d\Theta_{\mathrm{end}}=dE$ and

$$
\boxed{M(\alpha)=2\pi\frac{d}{d\alpha}\int_0^a W(\lambda,\lambda^{-1},1)\rho\,d\rho.}
$$

The radius $a$ is fixed in this derivative. This argument computes the required end [torque](../../../../../torque.md) along the prescribed deformation family; proving that a suitable end-only traction distribution sustains that family is unnecessary here.

For a [neo-Hookean solid](../../../../../neo-hookean-solid.md), the identity $\lambda-\lambda^{-1}=s$ gives $\lambda^2+\lambda^{-2}-2=s^2$. Therefore

$$
W=\frac\mu2\alpha^2\rho^2,\qquad E/L=\frac{\pi\mu a^4\alpha^2}{4},\qquad \boxed{M=\frac{\pi\mu a^4}{2}\alpha.}
$$

This is the signed [torque](../../../../../torque.md) in the twist direction; its magnitude is $\pi\mu a^4|\alpha|/2$. For the positive twist convention the signed value equals the magnitude.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
