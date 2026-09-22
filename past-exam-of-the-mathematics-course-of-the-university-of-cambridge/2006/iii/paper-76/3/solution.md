<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use reference cylindrical coordinates $(R,\Theta,Z)$ and current coordinates $(r,\theta,z)$. The prescribed map has $r=\lambda^{-1/2}R$, $\theta=\Theta+\alpha Z$ and $z=\lambda Z$. In the corresponding orthonormal cylindrical bases, differentiate physical line elements to obtain the [deformation gradient](../../../../../deformation-gradient.md)

$$
F=\begin{pmatrix}\lambda^{-1/2}&0&0\\0&\lambda^{-1/2}&\alpha R\lambda^{-1/2}\\0&0&\lambda\end{pmatrix},\qquad J=1.
$$

The radial direction is an eigenvector of the [right Cauchy-Green deformation tensor](../../../../../right-cauchy-green-deformation-tensor.md) with eigenvalue $\lambda^{-1}$. Its other block is

$$
\begin{pmatrix}\lambda^{-1}&\alpha R\lambda^{-1}\\\alpha R\lambda^{-1}&\lambda^2+\alpha^2R^2\lambda^{-1}\end{pmatrix}.
$$

Its trace is $s=\lambda^{-1}(1+\alpha^2R^2)+\lambda^2$ and its determinant is $\lambda$. Thus its eigenvalues solve $z^2-sz+\lambda=0$. The [principal stretches](../../../../../principal-stretch.md) are the positive square roots of these eigenvalues:

$$
\boxed{\lambda_1^2=\lambda^{-1},\qquad \lambda_{2,3}^2=\tfrac12\left(s\pm\sqrt{s^2-4\lambda}\right)}.
$$

Their product is one, independently checking [incompressibility](../../../../../incompressible-flow.md).

The [strain energy density](../../../../../strain-energy-density.md) $W$ is per reference volume, so stored energy per initial cylinder height is $\mathcal E(\alpha,\lambda)=2\pi\int_0^A W(\lambda_1,\lambda_2,\lambda_3)R\,dR$. The end rotation is $\alpha H$ and the current height is $\lambda H$, giving applied power per initial height $M\dot\alpha+N\dot\lambda$. For quasistatic reversible loading, equate this with $\dot{\mathcal E}$ for independent changes of $\alpha,\lambda$. This proves the [torque and axial force of a twisted incompressible cylinder](../../../../../torque-and-axial-force-of-a-twisted-incompressible-cylinder.md) formulas

$$
\boxed{M=2\pi\frac{\partial}{\partial\alpha}\int_0^A WR\,dR,\qquad N=2\pi\frac{\partial}{\partial\lambda}\int_0^A WR\,dR}.
$$

In the second derivative hold $\alpha$, the twist per initial length, fixed. Holding twist per current length instead would mix the generalized forces.

For the [Mooney-Rivlin solid](../../../../../mooney-rivlin-solid.md), compute invariants directly from $F$ rather than differentiating individual eigenvalue square roots:

$$
I_1=\lambda^2+2\lambda^{-1}+\alpha^2R^2\lambda^{-1},\qquad I_2=\lambda^{-2}+2\lambda+\alpha^2R^2\lambda^{-2}.
$$

The second identity follows from $I_2=\operatorname{tr}(F^TF)^{-1}$ when $J=1$. Retain the paper's minus sign on its $\mu_2$ term. Integrating $R$ and $R^3$ gives

$$
\mathcal E=\frac{\pi A^2}{2}\{\mu_1(\lambda^2+2\lambda^{-1}-3)-\mu_2(\lambda^{-2}+2\lambda-3)\}+\frac{\pi A^4\alpha^2}{4}(\mu_1\lambda^{-1}-\mu_2\lambda^{-2}).
$$

Consequently

$$
\boxed{M=\frac{\pi A^4\alpha}{2}(\mu_1\lambda^{-1}-\mu_2\lambda^{-2})},
$$



$$
\boxed{N=\pi A^2\{\mu_1(\lambda-\lambda^{-2})-\mu_2(1-\lambda^{-3})\}+\frac{\pi A^4\alpha^2}{4}(-\mu_1\lambda^{-2}+2\mu_2\lambda^{-3})}.
$$

As checks, untwisted unit stretch gives $M=N=0$, and setting $\mu_2=0$ recovers the [neo-Hookean solid](../../../../../neo-hookean-solid.md) formulas. A convention with a positive second-invariant coefficient corresponds to replacing this $\mu_2$ by its negative.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
