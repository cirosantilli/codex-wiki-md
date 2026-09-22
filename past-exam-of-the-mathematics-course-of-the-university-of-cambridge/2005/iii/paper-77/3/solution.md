<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In this continuation $\lambda$ measures eccentricity, not the viscosity ratio used in Question 2. Take $\epsilon\to0$ with $0\leq\lambda<1$ fixed. For the [nearly occluding sphere in a cylindrical tube](../../../../../nearly-occluding-sphere-in-a-cylindrical-tube.md), the narrow gap has thickness $H\sim\epsilon a$ and axial length $\ell\sim a\sqrt\epsilon$, obtained by balancing $h_0$ and $x^2/(2a)$. In the sphere frame the tangential velocity scale is $U$. The [lubrication approximation](../../../../../lubrication-theory.md) then gives the **gap scales**

$$
\boxed{|p_x|\sim\frac{\mu U}{a^2\epsilon^2},\qquad
|p-p_{\mathrm{far}}|\sim\frac{\mu U}{a\epsilon^{3/2}},\qquad
|\sigma_{xy}|\sim\frac{\mu U}{a\epsilon}.}
$$

The large local pressure excursion is distinct from the eventual net pressure jump. Away from the sphere the velocity varies across a radius $a$, so the far [Hagen-Poiseuille flow](../../../../../hagen-poiseuille-equation.md) has

$$
\boxed{|p_x|\sim\frac{\mu U}{a^2},\qquad|\sigma_{rx}|\sim\frac{\mu U}{a}.}
$$

These scales also show why the gap pressure can be much larger than its shear stress while the leading net jump can be smaller than that pressure.

Use $y=a-r$, so $y=0$ is the moving tube wall and $y=h$ is the locally stationary sphere. The [no-slip boundary conditions](../../../../../no-slip-boundary-condition.md) are $u(0)=-U$, $u(h)=0$. Integrating $\mu u_{yy}=p_x$, with pressure independent of $y$ to leading order, gives the [Couette-Poiseuille flow in a thin gap](../../../../../couette-poiseuille-flow-in-a-thin-gap.md)

$$
u(y)=\frac{p_x}{2\mu}y(y-h)+U\left(\frac yh-1\right),\qquad
q=\int_0^hu\,dy=-\frac{h^3}{12\mu}p_x-\frac{Uh}{2}.
$$

Differentiate at both surfaces and eliminate $p_x$ using this [moving-boundary lubrication flux](../../../../../moving-boundary-lubrication-flux.md):

$$
\boxed{\frac{\sigma_{xy}(0)}\mu=\frac{4U}h+\frac{6q}{h^2},\qquad
\frac{\sigma_{xy}(h)}\mu=-\frac{2U}h-\frac{6q}{h^2}.}
$$

The coordinate reversal means $\sigma_{rx}=-\sigma_{xy}$ at the tube wall.

At leading order $q$ is independent of $x$ in each angular strip, though it may depend on $\theta$. Both boundaries are stationary as shapes in the sphere frame and impermeable, so the integrated [continuity equation](../../../../../continuity-equation.md) is $q_x+a^{-1}(q_\theta^{\mathrm{circ}})_\theta=0$. The pressure changes along $x$ over $a\sqrt\epsilon$ but along the circumference over $a$. Thus circumferential velocity is only $O(U\sqrt\epsilon)$, and its flux is $O(Ua\epsilon^{3/2})$. Circumferential flux divergence is smaller than the possible leading axial divergence by a factor $\epsilon$. Consequently $q_x=0$ to the order needed. This is not an assumption of equal flux at different angular positions.

For fixed $\theta$ define the [lubrication resistance integrals for a nearly occluding sphere](../../../../../lubrication-resistance-integrals-for-a-nearly-occluding-sphere.md)

$$
J_n(\theta)=\int_{-\infty}^{\infty}\frac{dx}{h(\theta,x)^n}
=\sqrt{2a}\,h_0^{1/2-n}I_n.
$$

In particular, $J_1=\pi\sqrt{2a/h_0}$, $J_2=J_1/(2h_0)$ and $J_3=3J_1/(8h_0^2)$. The local pressure relation gives

$$
\int p_xdx=-12\mu qJ_3-6\mu UJ_2.
$$

A putative generic value $q=O(Uh_0)$ makes this jump $O(\mu U/(a\epsilon^{3/2}))$. However, the integrated wall shear in part (ii) is only $O(\mu Ua/\sqrt\epsilon)$, so the [force-free](../../../../../force-free.md) global balance permits a common net pressure jump only of order $\mu U/(a\sqrt\epsilon)$. The outer flow has circumferentially uniform pressures on both sides. Therefore the $O(\epsilon^{-3/2})$ pressure jump must cancel in every angular strip, not merely after angular averaging. The [pressure recovery condition in lubrication flow](../../../../../pressure-recovery-condition-in-lubrication-flow.md) determines

$$
-12\mu qJ_3-6\mu UJ_2=0,\qquad
\boxed{q=-\frac U2\frac{J_2}{J_3}=-\frac23Uh_0(\theta).}
$$

This explains how the leading-order part of the global force balance selects the local flux.

The total sphere-frame [volume flux](../../../../../volumetric-flow-rate.md) is now

$$
Q_{\mathrm{frame}}=a\int_0^{2\pi}q(\theta)d\theta
=-\frac43\pi\epsilon a^2U.
$$

Transforming back to the laboratory adds $\pi a^2U$, so $Q_{\mathrm{lab}}=\pi a^2U(1-4\epsilon/3)$ to this order. For physical pressure, [Hagen-Poiseuille flow](../../../../../hagen-poiseuille-equation.md) gives $Q_{\mathrm{lab}}=-\pi a^4p_x/(8\mu)$. Thus

$$
\boxed{-p_x=\frac{8\mu U}{a^2}\left(1-\frac43\epsilon\right)+o\left(\frac{\epsilon\mu U}{a^2}\right).}
$$

The printed positive expression is the pressure-drop gradient in the direction of the laboratory flow; the Poiseuille hint omits the minus sign when $p_x$ is read as the derivative of physical pressure. With the specified wall velocity $-U$, the laboratory flow is positive and its physical pressure gradient is negative.

Next insert the leading flux into the wall [shear stress](../../../../../shear-stress.md):

$$
\sigma_{xy}(0)=4\mu U\left(\frac1h-\frac{h_0}{h^2}\right),\qquad
\int\sigma_{xy}(0)dx=4\mu U(J_1-h_0J_2)=2\mu UJ_1.
$$

Let $\Delta p>0$ be the localized extra pressure drop, after subtracting the regular far Poiseuille gradient. Contributions outside the neck are only $O(\mu U/a)$ and are smaller than the $O(\epsilon^{-1/2})$ jump. Since $\sigma_{rx}=-\sigma_{xy}$, part (ii) gives $\pi a^2\Delta p=a\int\!\int\sigma_{xy}(0)dxd\theta$. Hence the **leading pressure drop** is

$$
\boxed{\Delta p\sim\sqrt{\frac2\epsilon}\frac{2\mu U}a
\int_0^{2\pi}\frac{d\theta}{\sqrt{1+\lambda\cos\theta}}.}
$$

For example, the concentric limit is $\Delta p\sim4\pi\mu U\sqrt{2/\epsilon}/a$. The integral grows as the minimum gap shrinks; the fixed-$\lambda<1$ qualification prevents treating a further near-contact limit as uniformly covered.

On the sphere the leading [shear stress](../../../../../shear-stress.md) is $\sigma_{xy}(h)=-2\mu U/h+4\mu Uh_0/h^2$, so

$$
\boxed{\int_{-\infty}^{\infty}\sigma_{xy}(h)dx
=-2\mu UJ_1+4\mu Uh_0J_2=0.}
$$

Positive and negative tangential stresses cancel within each angular strip. Thus the leading tangential resultant, and its leading torque contribution, vanish: negligible rotation is consistent with the [torque-free](../../../../../torque-free.md) condition. The shear is not zero pointwise, and the pressure forces are not zero. Pressure on a sphere cannot produce a torque about its centre because its normal is radial; its force contributions and the matched far pressure jump remain essential to the [force-free transport of a nearly occluding sphere](../../../../../force-free-transport-of-a-nearly-occluding-sphere.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
