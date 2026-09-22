<h1 id="37e/solution">Solution</h1>

↑ **Parent:** [37E](../37e.md)

For an axisymmetric flow without azimuthal velocity, define the [Stokes streamfunction](../../../../../stokes-streamfunction.md) by

$$
\boxed{u_R=\frac{\Psi_\theta}{R^2\sin\theta},\qquad u_\theta=-\frac{\Psi_R}{R\sin\theta},\qquad u_\phi=0.}
$$

These formulas enforce incompressibility. The only nonzero curl component is $R^{-1}[\partial_R(Ru_\theta)-\partial_\theta u_R]$. Substitution gives

$$
\nabla\times u=\left(0,0,-\frac{D^2\Psi}{R\sin\theta}\right),\qquad
D^2=\partial_R^2+\frac{\sin\theta}{R^2}\partial_\theta\left(\frac1{\sin\theta}\partial_\theta\right).
$$

Curling the [Stokes flow](../../../../../stokes-flow-split.md) equations eliminates pressure and gives $\nabla^2(\nabla\times u)=0$. For an azimuthal field, its vector Laplacian is the scalar Laplacian minus $1/(R^2\sin^2\theta)$; applying that operator to $-D^2\Psi/(R\sin\theta)$ gives $-D^2(D^2\Psi)/(R\sin\theta)$. Hence the streamfunction equation is $\boxed{D^2D^2\Psi=0}$.

For the proposed sphere solution put $f(R)=R^2-3aR/2+a^3/(2R)$, so $\Psi=(U/2)f(R)\sin^2\theta$. Its velocity is

$$
u_R=U\cos\theta\left(1-\frac{3a}{2R}+\frac{a^3}{2R^3}\right),\qquad
u_\theta=-U\sin\theta\left(1-\frac{3a}{4R}-\frac{a^3}{4R^3}\right).
$$

Both components vanish at $R=a$ and tend to the components of $Ue_z$ at infinity. Also $D^2\Psi=(U/2)(f''-2f/R^2)\sin^2\theta=(3Ua/(2R))\sin^2\theta$, and applying $D^2$ once more gives zero. This verifies the differential equation and both physical boundary conditions.

For a sphere translating upward through otherwise stationary fluid, subtract the uniform background in the sphere frame and reverse its far-flow direction. Its leading disturbance is the upward [Stokeslet](../../../../../stokeslet.md)

$$
u(R)=\frac{3aU}{4R}(I+\widehat R\widehat R^{\mathsf T})e_z+O(Ua^3/R^3).
$$

Place an image at $z=+d$ with the **opposite**, downward velocity $-U$, while the real sphere is at $z=-d$. The sum has $u_z$ odd under $z\mapsto-z$ and $u_r$ even. Thus at $z=0$, $u_z=0$ and $\partial_z u_r=0$; moreover $\partial_r u_z=0$. The tangential stress $\sigma_{rz}=\mu(\partial_z u_r+\partial_r u_z)$ is therefore zero, as required by the [stress-free boundary condition](../../../../../stress-free-boundary-condition.md).

At a point on the plane with radial coordinate $r$, the real Stokeslet gives $u_r=3aUrd/[4(r^2+d^2)^{3/2}]$. The image gives the same radial contribution, so

$$
\boxed{u_r(r,0)=\frac{3aUrd}{2(r^2+d^2)^{3/2}}+O\!\left(U\frac{a^2}{d^2}\right)\quad(r/d\text{ fixed}).}
$$

The surface flow is outward. Although the isolated-sphere dipole term is only $O(U(a/d)^3)$, the **next correction is $O(U(a/d)^2)$**: the image's velocity at the real sphere is downward and of size $3aU/(4d)$, so satisfying the real sphere's prescribed velocity requires a relative $O(a/d)$ correction to its Stokeslet strength. Since the leading surface flow is $O(Ua/d)$, the first reflection already changes it at the displayed second order. Ignoring this boundary-interaction correction would give the wrong next power.

## ↑ Ancestors (10)

1. [37E](../37e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
