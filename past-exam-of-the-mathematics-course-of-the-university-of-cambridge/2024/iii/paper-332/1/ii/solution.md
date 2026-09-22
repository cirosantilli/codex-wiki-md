<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $z$ measure height above the sponge. Under the [long-wave approximation](../../../../../../long-wave-approximation.md), [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) gives $p_x=\rho gH_x$, and the horizontal balance for [viscous fluid flow](../../../../../../viscous-fluid-flow-split.md) is

$$
\mu u_{zz}=\rho gH_x.
$$

The [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) $u(0)=0$ and [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) $u_z(H)=0$ give

$$
u=\frac{\rho g}{\mu}H_x
\left(\frac{z^2}{2}-Hz\right).
$$

Integrating this [lubrication theory](../../../../../../lubrication-theory.md) profile gives the horizontal [volume flux](../../../../../../volumetric-flow-rate.md) per unit span

$$
q=\int_0^H u\,dz
=-AH^3H_x,
\qquad
A=\frac{\rho g}{3\mu}.
$$

Local [mass conservation](../../../../../../mass-conservation.md) includes the downward loss found in part i:

$$
H_t+q_x=-DH^{1-\beta}.
$$

Consequently the required nonlinear [partial differential equation](../../../../../../partial-differential-equation-split.md) is

$$
\boxed{H_t=A(H^3H_x)_x-DH^{1-\beta}}.
$$

If the imposed inlet flux is $Q_0t^\alpha$ and the moving front is $x=x_N(t)$, sufficient [boundary conditions](../../../../../../boundary-condition.md) are

$$
-AH(0,t)^3H_x(0,t)=Q_0t^\alpha,
$$



$$
H(x_N(t),t)=0,
\qquad
q(x_N(t),t)=0.
$$

For a current released onto a dry substrate one also takes the [initial condition](../../../../../../initial-condition.md) $H(x,0)=0$ away from the source. The front position is part of this [moving-boundary problem](../../../../../../moving-boundary-problem.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
