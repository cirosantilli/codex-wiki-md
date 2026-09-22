<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take positive $x$ in the snail's direction of travel, and let $y$ measure height above the rigid plane. The wave moves at laboratory [velocity](../../../../../velocity.md) $U-V$. In the wave frame the plane's horizontal [velocity](../../../../../velocity.md) is $V-U$ and the foot's is $V$. The foot is stationary as a shape, so its material [velocity](../../../../../velocity.md) is tangent to $y=h(x)$: to leading [lubrication theory](../../../../../lubrication-theory.md) order its components are $(V,Vh_x)$. Apply the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) to both surfaces.

The leading [Stokes flow](../../../../../stokes-flow-split.md) equations are $p_y=0$ and $\mu u_{yy}=p_x$. Their solution is the local [Couette-Poiseuille flow](../../../../../couette-poiseuille-flow.md)

$$
\boxed{u(x,y)=V-U+\frac{Uy}{h(x)}+\frac{p_x}{2\mu}y(y-h).}
$$

The normal-velocity condition on each steady surface and [incompressibility](../../../../../incompressible-flow.md) make the wave-frame flux independent of $x$. Integrating the [velocity](../../../../../velocity.md) gives

$$
q=h\left(V-\frac U2\right)-\frac{h^3p_x}{12\mu}.
$$

Put $C=V-U/2$. Periodicity of [pressure](../../../../../pressure.md) gives $0=\int_0^Lp_xdx=12\mu(CI_2-qI_3)$, and hence

$$
\boxed{q=C\frac{I_2}{I_3},\qquad
p_x=12\mu\left(\frac C{h^2}-\frac q{h^3}\right),\qquad
I_j=\int_0^Lh^{-j}dx.}
$$

The shear traction exerted by the fluid on the plane, positive in the $x$ direction, is

$$
\boxed{\tau_0=\mu u_y(x,0)=\frac{\mu U}{h}-\frac h2p_x
=\frac{\mu(4U-6V)}h+\frac{6\mu q}{h^2}.}
$$

The snail is force-free horizontally: its gait consists of internal motion and it has no externally applied horizontal drive. Uniform locomotion therefore requires zero net horizontal fluid [force](../../../../../force.md) on the foot per wavelength. The stresses on opposite periodic fluid faces cancel, so horizontal momentum balance also makes the net [force](../../../../../force.md) on the plane zero. Thus

$$
0=\int_0^L\tau_0dx=\mu(4U-6V)I_1+6\mu qI_2.
$$

Substitution of $q$ proves the [lubrication model of a crawling snail](../../../../../lubrication-model-of-a-crawling-snail.md):

$$
\boxed{U=\frac{6(1-\alpha)}{4-3\alpha}V,\qquad
\alpha=\frac{I_2^2}{I_1I_3}.}
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) applied to $h^{-1/2}$ and $h^{-3/2}$ gives $0<\alpha\leq1$, with equality exactly for a uniform gap. Thus the denominator is positive, and a nonuniform waveform gives forward motion; the flat gap gives $U=0$.

For the sinusoidal shape, the given integrals yield

$$
I_1=\frac{L}{h_0\sqrt{1-A^2}},\qquad
I_2=\frac{L}{h_0^2(1-A^2)^{3/2}},\qquad
I_3=\frac{L(1+A^2/2)}{h_0^3(1-A^2)^{5/2}}.
$$

Therefore $\alpha=1/(1+A^2/2)$ and

$$
\boxed{U=\frac{3A^2}{1+2A^2}V.}
$$

For small amplitude, $U\sim3A^2V$: the leading locomotion is quadratic, and there is no propulsion from a flat foot. As $A\to1^-$, $U\to V$, so the wave becomes nearly stationary in the laboratory frame while the snail advances relative to it. However, the minimum gap tends to zero; finite speed in this limit does not imply finite dissipation, and $A=1$ itself is excluded by the noncontact model.

For the general waveform, use the mechanical work identity for [viscous dissipation](../../../../../viscous-dissipation.md). [Pressure](../../../../../pressure.md) does no boundary work because the boundary motion is tangential in the wave frame. The plane's [velocity](../../../../../velocity.md) is constant, and its total [force](../../../../../force.md) is zero, so it contributes zero net work. The upper boundary supplies, at leading lubrication order,

$$
\Phi=\mu V\int_0^Lu_y(x,h)dx
=V\left(\mu UI_1+\frac12\int_0^Lhp_xdx\right).
$$

The zero plane-force relation is $\mu UI_1=\tfrac12\int hp_xdx$. Consequently

$$
\boxed{\Phi=2\mu UVI_1.}
$$

As a direct check, integrating the squared shear rate gives $\Phi=\int_0^L[\mu U^2/h+h^3p_x^2/(12\mu)]dx=\mu I_1[U^2+12C^2(1-\alpha)]$, which reduces to the same result using the force-free speed relation. Zero horizontal [force](../../../../../force.md) on the foot does not mean zero gait work: the tangential material [velocity](../../../../../velocity.md) along its sloping surface includes vertical motion.

For prescribed speed $U>0$ and sinusoidal shape, eliminate $V=U(1+2A^2)/(3A^2)$ to obtain

$$
\Phi(A)=\frac{2\mu LU^2}{3h_0}\frac{1+2A^2}{A^2\sqrt{1-A^2}}.
$$

Writing $y=A^2$, the logarithmic derivative of the amplitude-dependent factor is

$$
\frac2{1+2y}-\frac1y+\frac1{2(1-y)}=0
\quad\Longleftrightarrow\quad2y^2+3y-2=0.
$$

The only root in $0<y<1$ is $y=1/2$. The dissipation diverges at both endpoints, so this is the global minimum and gives the [optimal sinusoidal waveform for viscous snail locomotion](../../../../../optimal-sinusoidal-waveform-for-viscous-snail-locomotion.md):

$$
\boxed{A_{\rm opt}=\frac1{\sqrt2},\qquad V_{\rm opt}=\frac43U,\qquad
\Phi_{\min}=\frac{8\sqrt2}{3}\frac{\mu LU^2}{h_0}.}
$$

The magically driven flat glider has simple [Couette flow](../../../../../couette-flow.md) $u=Uy/h_0$ in the laboratory frame, and dissipation $\Phi_{\rm glide}=\mu LU^2/h_0$ per wavelength. Hence

$$
\boxed{\Phi_{\min}/\Phi_{\rm glide}=8\sqrt2/3.}
$$

The comparison is at the same $U$, mean thickness $h_0$ and wavelength $L$; the flat glider is externally propelled, whereas the snail must power its internal waveform.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
