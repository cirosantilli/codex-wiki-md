<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the [shallow-water approximation](../../../../../shallow-water-approximation.md), let the vertical scale be much smaller than the horizontal scale, so vertical acceleration is negligible and [pressure](../../../../../pressure.md) is hydrostatic. Assume constant [density](../../../../../density.md), a flat impermeable bottom, a [free surface](../../../../../free-surface.md) under constant atmospheric [pressure](../../../../../pressure.md), and a horizontally moving column with no leading-order vertical shear. Neglect friction. Taking the bottom at $z=0$, [hydrostatic pressure](../../../../../hydrostatic-pressure.md) is $p=p_a+\rho g(h-z)$, so its horizontal gradient is independent of $z$. The horizontal momentum equations are therefore

$$
\frac{D_Hu}{Dt}=-gh_x,\qquad \frac{D_Hv}{Dt}=-gh_y,\qquad \frac{D_H}{Dt}=\partial_t+u\partial_x+v\partial_y.
$$

Integrating [incompressibility](../../../../../incompressible-flow.md) from the bottom to the [free surface](../../../../../free-surface.md), using zero bottom vertical [velocity](../../../../../velocity.md) and the surface kinematic condition $w=h_t+uh_x+vh_y$, gives

$$
\boxed{h_t+\partial_x(hu)+\partial_y(hv)=0.}
$$

Together these are the nonrotating [shallow water equations](../../../../../shallow-water-equations.md).

Rotation with angular [velocity](../../../../../velocity.md) $f\hat{\boldsymbol z}/2$ adds [Coriolis force](../../../../../coriolis-force.md) terms $-fv$ and $+fu$ to the left sides of the $u$ and $v$ equations, respectively. The centrifugal potential is absorbed into the background [pressure](../../../../../pressure.md) and effective gravity. Thus

$$
D_Hu-fv=-gh_x,\qquad D_Hv+fu=-gh_y.
$$

Write $\zeta=v_x-u_y$ and $d=u_x+v_y$. Taking the horizontal curl, including the derivatives of the advecting [velocity](../../../../../velocity.md), yields

$$
D_H\zeta=-(\zeta+f)d.
$$

For example the curl of the [Coriolis force](../../../../../coriolis-force.md) contribution is $fd$, and the curl of nonlinear [advection](../../../../../advection.md) supplies $\zeta d$. Since $q_a=f+\zeta$ and $D_Hh=-hd$, division gives

$$
\boxed{\frac{D_H}{Dt}\left(\frac{q_a}{h}\right)=\frac{-q_a d}{h}+\frac{q_a hd}{h^2}=0.}
$$

This is exact [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md) conservation within the rotating [shallow water equations](../../../../../shallow-water-equations.md).

For the [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md), take a horizontal scale $L$, speed $U$, mean depth $H$, and slow time $L/U$. Require small [Rossby number](../../../../../rossby-number.md) $\mathrm{Ro}=U/(|f|L)\ll1$ and small surface departure $\eta=h-H$. Introduce the [Rossby deformation radius](../../../../../rossby-deformation-radius.md) $L_R=\sqrt{gH}/|f|$ and [Burger number](../../../../../burger-number.md) $\mathrm{Bu}=L_R^2/L^2=O(1)$. [Geostrophic balance](../../../../../geostrophic-balance.md) gives $g\eta/L\sim|f|U$, hence $\eta/H\sim\mathrm{Ro}/\mathrm{Bu}\ll1$. The [Froude number](../../../../../froude-number.md) is $U/\sqrt{gH}=\mathrm{Ro}/\sqrt{\mathrm{Bu}}\ll1$. These assumptions select slow balanced motion, with fast gravity-wave transients absent at leading order.

Define the [quasi-geostrophic streamfunction](../../../../../quasi-geostrophic-streamfunction.md) by $\psi=g\eta/f$. The leading [geostrophic flow](../../../../../geostrophic-flow.md) is $(u_g,v_g)=(-\psi_y,\psi_x)$, which is horizontally nondivergent. Expanding the exact [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md) gives

$$
\frac{f+\zeta}{H+\eta}=\frac{f}{H}+\frac{1}{H}\left(\nabla_H^2\psi-\frac{\psi}{L_R^2}\right)+\text{higher-order terms}.
$$

The correction is smaller than $f/H$ by $O(\mathrm{Ro})$. Advecting it by the leading [geostrophic flow](../../../../../geostrophic-flow.md), while the constant leading term has zero gradient, gives

$$
\boxed{Q=f+\nabla_H^2\psi-L_R^{-2}\psi,\qquad Q_t+J_{xy}(\psi,Q)=0,\qquad J_{xy}(A,B)=A_xB_y-A_yB_x.}
$$

Here [potential-vorticity conservation](../../../../../potential-vorticity-conservation.md) means that $Q$ is carried unchanged by the leading horizontal trajectories. [Potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) means solving the elliptic equation $(\nabla_H^2-L_R^{-2})\psi=Q-f$, with appropriate boundary or decay conditions, to recover $\psi$ and thus the [velocity](../../../../../velocity.md). Conservation evolves the scalar field; inversion obtains its [velocity](../../../../../velocity.md) field.

For a mean current $U(y)=-\bar\psi_y$, substitute $Q=\bar Q+Q'$ and $\psi=\bar\psi+\psi'$ into [potential-vorticity conservation](../../../../../potential-vorticity-conservation.md). Retaining first-order terms gives

$$
\boxed{Q'_t+UQ'_x+\bar Q_y\psi'_x=0.}
$$

Let $\Delta Q=\bar Q(0^+)-\bar Q(0^-)>0$. Differentiating the mean inversion relation gives $\bar Q_y=-U''+L_R^{-2}U$. Away from $y=0$ this is zero, so decay at both infinities gives $U=U_0e^{-|y|/L_R}$. A [velocity](../../../../../velocity.md) jump would introduce a derivative of a delta function, absent from $\bar Q_y$, so $U$ is continuous. Integrating through zero now gives $-[U']=\Delta Q$, and therefore

$$
\boxed{U_0=\frac{L_R\Delta Q}{2},\qquad U(y)=\frac{L_R\Delta Q}{2}e^{-|y|/L_R}.}
$$

For the regular interfacial [normal mode](../../../../../normal-mode.md) $\psi'=\phi(y)e^{ik(x-ct)}$, the linear equation reads

$$
(U-c)\bigl(\phi''-(k^2+L_R^{-2})\phi\bigr)+\Delta Q\,\delta(y)\phi=0.
$$

In each region, choose zero perturbation [potential vorticity](../../../../../potential-vorticity.md), giving $\phi''-(k^2+L_R^{-2})\phi=0$. This supplies a regular solution even if $U=c$ at isolated locations away from the interface. Continuity and decay require $\phi=Ae^{-\gamma|y|}$, where $\gamma=\sqrt{k^2+L_R^{-2}}$. Integrating the equation across zero gives

$$
(U_0-c)[\phi']+\Delta Q\phi(0)=0.
$$

Since $[\phi']=-2\gamma A$, the nonzero [normal mode](../../../../../normal-mode.md) has

$$
\boxed{c=U_0-\frac{\Delta Q}{2\gamma}=U_0\left(1-\sqrt{\frac{L_R^{-2}}{k^2+L_R^{-2}}}\right),\qquad \phi=Ae^{-\gamma|y|}.}
$$

This [potential-vorticity step edge wave](../../../../../potential-vorticity-step-edge-wave.md) is an interfacial [Rossby wave](../../../../../rossby-wave.md). Displacing the [potential vorticity](../../../../../potential-vorticity.md) jump creates alternating anomalies; their inverted [velocity](../../../../../velocity.md) displaces the interface further with an intrinsic propagation opposite to the positive mean current. The mechanism requires a nonzero jump, or more generally a gradient, of the mean [potential vorticity](../../../../../potential-vorticity.md). It does not require planetary variation of $f$. Reversing the jump reverses the intrinsic propagation; setting the jump to zero removes this interfacial restoring mechanism.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
