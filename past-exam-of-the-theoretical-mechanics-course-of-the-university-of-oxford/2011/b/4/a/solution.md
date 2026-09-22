<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R(t)$ rotate [vectors](../../../../../vector.md) from the rotating frame to the inertial frame. For any rotating-frame [vector](../../../../../vector.md) $\mathbf a$, differentiating $R\mathbf a$ adds $R(\boldsymbol\Omega\times\mathbf a)$ to $R\dot{\mathbf a}$. Thus an inertial particle [velocity](../../../../../velocity.md) is $R(\mathbf u+\boldsymbol\Omega\times\mathbf x)$, and, for constant [angular velocity](../../../../../angular-velocity.md), its [acceleration](../../../../../acceleration.md) is

$$
R\left[\frac{D\mathbf u}{Dt}+2\boldsymbol\Omega\times\mathbf u+\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf x)\right].
$$

Insert this into the inertial [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid-split.md) and express [forces](../../../../../force-split.md) in the rotating coordinates. This gives

$$
\boxed{\frac{D\mathbf u}{Dt}+2\boldsymbol\Omega\times\mathbf u+\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf x)=-\rho^{-1}\nabla p+\mathbf g.}
$$

The additional terms are the [Coriolis acceleration](../../../../../coriolis-acceleration.md) and the centripetal term associated with frame rotation. There is no angular-[acceleration](../../../../../acceleration.md) term because $\boldsymbol\Omega$ is constant.

Write the conservative [body force](../../../../../body-force.md) as $\mathbf g=-\nabla\Phi_g$. The supplied [vector](../../../../../vector.md) identity gives $\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf x)=-\tfrac12\nabla|\boldsymbol\Omega\times\mathbf x|^2$. For constant [density](../../../../../density.md), define

$$
\boxed{P=p+\rho\Phi_g-\frac\rho2|\boldsymbol\Omega\times\mathbf x|^2.}
$$

Moving the centrifugal and conservative terms to the right then gives $\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u+2\boldsymbol\Omega\times\mathbf u=-\rho^{-1}\nabla P$. Only the [gradient](../../../../../gradient.md) of this reduced [pressure](../../../../../pressure-split.md) matters, so an additive spatial constant is immaterial.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
