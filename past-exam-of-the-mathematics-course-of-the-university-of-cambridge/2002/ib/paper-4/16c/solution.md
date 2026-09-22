<h1 id="16c/solution">Solution</h1>

↑ **Parent:** [16C](../16c.md)

Use the standard constant-density [incompressible flow](../../../../../incompressible-flow.md) model, with conservative body force. Write $\mathbf u=(u,v,0)$ independent of $z$, and $\omega=v_x-u_y$. Differentiate the $y$-momentum [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) with respect to $x$ and subtract the $y$-derivative of the $x$-momentum equation. Mixed pressure derivatives and the curl of a conservative body force cancel, giving

$$
\omega_t+u\omega_x+v\omega_y+(u_x+v_y)\omega=0.
$$

The last term vanishes by [incompressibility](../../../../../incompressible-flow.md), so the material derivative of [vorticity](../../../../../vorticity.md) is zero. Thus **$D\omega/Dt=0$**. [Incompressibility](../../../../../incompressible-flow.md) is important: inviscidness alone does not suffice; in a compressible barotropic planar flow the equation is $D\omega/Dt=-\omega\nabla\cdot\mathbf u$, conserving $\omega/\rho$ instead.

Take vortex strength $\kappa$ to denote [circulation](../../../../../circulation-physics.md), positive counterclockwise. A [point vortex](../../../../../line-vortex.md) at $\mathbf x_0$ generates

$$
\mathbf u(\mathbf x)=\frac{\kappa}{2\pi}\frac{J(\mathbf x-\mathbf x_0)}{|\mathbf x-\mathbf x_0|^2},\qquad J(x,y)=(-y,x).
$$

It has zero [vorticity](../../../../../vorticity.md) away from its core, with circulation $\kappa$ around the core. Each vortex moves with the other's regular induced [velocity](../../../../../velocity.md), not its own singular field. With $\mathbf d=\mathbf x_1-\mathbf x_2$,

$$
\dot{\mathbf x}_1=\frac{\kappa_2}{2\pi|\mathbf d|^2}J\mathbf d,\qquad \dot{\mathbf x}_2=-\frac{\kappa_1}{2\pi|\mathbf d|^2}J\mathbf d.
$$

Multiplication by the two strengths proves $\dot{\mathbf q}=\kappa_1\dot{\mathbf x}_1+\kappa_2\dot{\mathbf x}_2=0$. Also $\dot{\mathbf d}=(\kappa_1+\kappa_2)J\mathbf d/(2\pi|\mathbf d|^2)$, so $d|\mathbf d|^2/dt=2\mathbf d\cdot\dot{\mathbf d}=0$.

For equal strengths $\kappa$ and the specified initial positions, $\mathbf q=0$ and $|\mathbf d|=2a$. The [motion of two point vortices](../../../../../motion-of-two-point-vortices.md) is rotation with angular [velocity](../../../../../velocity.md) $\Omega_v=\kappa/(4\pi a^2)$:

$$
\boxed{\mathbf x_1(t)=a(\cos\Omega_vt,\sin\Omega_vt),\qquad \mathbf x_2(t)=-\mathbf x_1(t).}
$$

Negative circulation reverses the rotation. If vortex strength is defined instead as the coefficient of $1/r$ [velocity](../../../../../velocity.md), absorb the factor $2\pi$ consistently into its definition.

## ↑ Ancestors (10)

1. [16C](../16c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
