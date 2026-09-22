<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Linearize about rest, with the equilibrium [forces](../../../../../force-split.md) already absorbed in the reduced [pressure](../../../../../pressure-split.md). The quadratic convective [acceleration](../../../../../acceleration.md) drops out. Since $\mathbf k\times(u\mathbf i+v\mathbf j+w\mathbf k)=-v\mathbf i+u\mathbf j$, the component equations are

$$
\boxed{u_t-2\Omega v=-P_x/\rho,\qquad v_t+2\Omega u=-P_y/\rho,\qquad w_t=-P_z/\rho,\qquad u_x+v_y+w_z=0.}
$$

The scan prints $v_w$ in the [continuity equation](../../../../../continuity-equation.md); **the [derivative](../../../../../derivative.md) required by [incompressibility](../../../../../incompressible-flow.md) is $v_y$**.

To eliminate [pressure](../../../../../pressure-split.md), put $\zeta=v_x-u_y$ and $\nabla_h^2=\partial_x^2+\partial_y^2$. Taking the vertical component of the [curl](../../../../../curl.md) of [momentum](../../../../../momentum-split.md) gives

$$
\zeta_t+2\Omega(u_x+v_y)=0,\qquad\text{so}\qquad\zeta_t=2\Omega w_z.
$$

Taking horizontal [divergence](../../../../../divergence.md) of [momentum](../../../../../momentum-split.md) and substituting continuity gives

$$
\rho^{-1}\nabla_h^2P=w_{zt}+2\Omega\zeta.
$$

Differentiate this in $z$ and use $P_z/\rho=-w_t$:

$$
\partial_t(\nabla^2w)+2\Omega\zeta_z=0.
$$

One more time [derivative](../../../../../derivative.md), followed by the [vorticity](../../../../../vorticity-split.md) relation, yields the [Poincaré equation for inertial waves](../../../../../poincare-equation-for-inertial-waves.md)

$$
\boxed{\partial_t^2(\nabla^2w)+4\Omega^2w_{zz}=0.}
$$

This derivation retains all three [velocity](../../../../../velocity.md) components, including the transverse component coupled by rotation.

## ↑ Ancestors (13)

1. [B](../b.md)
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
