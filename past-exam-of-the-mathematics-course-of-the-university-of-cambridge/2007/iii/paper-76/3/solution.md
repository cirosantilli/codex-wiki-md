<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $c=a^2-a_0^2$ and use reference cylindrical coordinates $(\rho,\Theta,Z)$ and current coordinates $(r,\theta,z)$. The [deformation map](../../../../../deformation-map.md) is $r=\sqrt{\rho^2+c}$, $\theta=\Theta+\alpha Z$, $z=Z$. In the associated orthonormal bases its [deformation gradient](../../../../../deformation-gradient.md) is

$$
F=\begin{pmatrix}\rho/r&0&0\\0&r/\rho&\alpha r\\0&0&1\end{pmatrix}.
$$

Its [determinant](../../../../../determinant.md) is one, as required by [incompressibility](../../../../../incompressible-flow.md). The radial [principal stretch](../../../../../principal-stretch.md) is $\lambda_0=\rho/r$. The other two squared [principal stretches](../../../../../principal-stretch.md) are the [eigenvalues](../../../../../eigenvalue.md) of the tangential-axial block of $FF^T$:

$$
\begin{pmatrix}(r/\rho)^2+\alpha^2r^2&\alpha r\\\alpha r&1\end{pmatrix}.
$$

Writing $K=(r/\rho)^2+\alpha^2r^2+1$, they are

$$
\boxed{\lambda_\pm^2=\frac{K\pm\sqrt{K^2-4(r/\rho)^2}}2,\qquad\lambda_0=\frac{\rho}{r}.}
$$

The positive square roots give $\lambda_\pm$, and $\lambda_0\lambda_+\lambda_-=1$.

The [strain energy density](../../../../../strain-energy-density.md) is per reference volume, so the energy per height is

$$
E(a,\alpha)=2\pi\int_{a_0}^{b_0}\rho W(\lambda_0,\lambda_+,\lambda_-)\,d\rho.
$$

The work rates per height are $M\dot\alpha$ from the end [torque](../../../../../torque.md) and $2\pi a\,p\dot a$ from the inner pressure. The outer surface contributes no work because it is traction free, and the fixed height has zero axial work. Thus the [virtual work](../../../../../virtual-work.md) identities for [twist and inflation of an incompressible tube](../../../../../twist-and-inflation-of-an-incompressible-tube.md) are

$$
\boxed{M=2\pi\frac{\partial}{\partial\alpha}\int_{a_0}^{b_0}\rho W\,d\rho,\qquad p(a)=\frac1a\frac{\partial}{\partial a}\int_{a_0}^{b_0}\rho W\,d\rho.}
$$

For a [neo-Hookean solid](../../../../../neo-hookean-solid.md), an irrelevant energy constant can be omitted:

$$
W=\frac\mu2\left(\frac{\rho^2}{r^2}+\frac{r^2}{\rho^2}+\alpha^2r^2+1\right).
$$

Differentiating under the finite integral gives

$$
p=\mu\int_{a_0}^{b_0}\rho\left[\frac1{\rho^2}-\frac{\rho^2}{(\rho^2+c)^2}+\alpha^2\right]\,d\rho.
$$

An antiderivative divided by $\mu$ is $\log\rho-\tfrac12\log(\rho^2+c)-c/[2(\rho^2+c)]+\alpha^2\rho^2/2$. With $b^2=b_0^2+c$, the [neo-Hookean tube pressure under twist and inflation](../../../../../neo-hookean-tube-pressure-under-twist-and-inflation.md) is therefore

$$
\boxed{p(a)=\mu\log\frac{b_0a}{a_0b}+\frac\mu2\left(\frac{b_0^2}{b^2}-\frac{a_0^2}{a^2}\right)+\frac{\mu\alpha^2}{2}(b_0^2-a_0^2).}
$$

It vanishes for an untwisted undeformed tube, and the twist contributes the last term at fixed radii.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
