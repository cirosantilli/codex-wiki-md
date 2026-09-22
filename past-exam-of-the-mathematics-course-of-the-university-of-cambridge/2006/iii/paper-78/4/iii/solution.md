<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\epsilon=1-\alpha\ll1$, and use local distance $\rho=a\theta$ from the closest pole. The gap is

$$
h\simeq\Delta\left(\epsilon+\frac{\theta^2}{2}\right)
=h_0+\frac{\rho^2}{2R},\qquad h_0=\epsilon\Delta,\quad R\simeq\frac{a^2}{\Delta}.
$$

Horizontal rotation has nonzero wall speed $V_s\sim|\Omega'|a$ at this pole. In the broad region with $h=O(\Delta)$, shear is $O(\mu|\Omega'|a/\Delta)$, the area is $O(a^2)$ and the lever arm is $O(a)$. Its [torque](../../../../../../torque.md) is therefore $O(\mu|\Omega'|a^4/\Delta)$. The smallest gap patch has radius $O(a\sqrt\epsilon)$ and area $O(a^2\epsilon)$; its shear is $O(\mu|\Omega'|a/(\epsilon\Delta))$. It gives the same bounded [torque](../../../../../../torque.md) scale.

These are the two estimates requested in the paper. **They omit an intermediate annulus, so the printed uniform $O(\mu|\Omega'|a^4/\Delta)$ assertion is not correct as $\epsilon\to0$.** For $a\sqrt\epsilon\ll\rho\ll a$, $h\sim\Delta\rho^2/a^2$. An annular shear-torque contribution scales as

$$
dG\sim a\frac{\mu V_s}{h}\,2\pi\rho\,d\rho
\sim\frac{\mu|\Omega'|a^4}{\Delta}\frac{d\rho}{\rho}.
$$

Integrating between the inner and outer scales produces $\log(1/\epsilon)$.

A [viscous dissipation](../../../../../../viscous-dissipation.md) lower bound makes this conclusion independent of possible signs of local tractions. A fluid [velocity](../../../../../../velocity.md) changing by $V_s$ between two no-slip walls dissipates at least $\mu V_s^2/h$ per unit area, by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in the cross-gap coordinate. The lubrication [velocity](../../../../../../velocity.md) profile gives more explicitly

$$
\int_0^h\mu|\partial_z u|^2dz
=\frac{\mu|v_s|^2}{h}+\frac{h^3|\nabla p|^2}{12\mu},
$$

with no cross term. The second term is nonnegative. Thus the annulus entails a logarithmic divergence in total power and hence in $|G'|$, since the centre is held fixed and all boundary work is $G'\Omega'$.

The [horizontal rotation in a nearly touching spherical shell](../../../../../../horizontal-rotation-in-a-nearly-touching-spherical-shell.md) calculation also gives the corrected [force](../../../../../../force.md) scale. Choose local $x$ along $v_s$ and put $V_s=a\Omega'$ with its signed value. At leading order the stationary-gap [Reynolds lubrication equation](../../../../../../reynolds-equation.md) is

$$
\nabla\cdot(h^3\nabla p)=6\mu V_s\partial_xh.
$$

For $h=h_0+(x^2+y^2)/(2R)$ it has the particular [pressure](../../../../../../pressure.md)

$$
p=-\frac{6\mu V_s}{5}\frac{x}{h^2},
$$

which satisfies the equation by direct differentiation. The [pressure](../../../../../../pressure.md) itself gives no [torque](../../../../../../torque.md) about the centre of an exactly spherical inner body, because its normal is radial. It does contribute to tangential shear through the [pressure](../../../../../../pressure.md) gradient.

For any fixed local outer cutoff, the logarithmically divergent integrals are

$$
I_1=\int\frac{dA}{h}\sim2\pi R\log(1/\epsilon),\qquad
I_2=\int\frac{x^2}{h^2}dA\sim2\pi R^2\log(1/\epsilon).
$$

The resisting tangential [traction](../../../../../../traction.md) is $\mu V_s/h+(h/2)p_x$. Integration by parts gives [torque](../../../../../../torque.md) magnitude $a\mu|V_s|(I_1+3I_2/(5R))$ to logarithmic order. Consequently, at leading order in $\Delta/a$,

$$
\boxed{|G'|\sim\frac{16\pi}{5}\frac{\mu|\Omega'|a^4}{\Delta}\log\frac1\epsilon.}
$$

The strict corrected order is $\Theta((\mu|\Omega'|a^4/\Delta)\log(1/\epsilon))$; the paper's scale is the bounded contribution of each of its two nominated regions, not the full asymptotic answer.

For the horizontal [force](../../../../../../force.md), [pressure](../../../../../../pressure.md) dominates shear by a factor $a/\Delta$. Its horizontal projection on the inner sphere has normal component $n_x\simeq x/a$, giving $|F_p|\sim(6\mu|V_s|/(5a))I_2$. Hence the required holding-force magnitude is

$$
\boxed{|F'|\sim\frac{12\pi}{5}\frac{\mu|\Omega'|a^4}{\Delta^2}\log\frac1\epsilon.}
$$

The broad region and smallest patch each supply $O(\mu|\Omega'|a^4/\Delta^2)$; the intermediate annulus again supplies the extra logarithm. The shear [force](../../../../../../force.md) is smaller by $\Delta/a$. These expressions assume the completely filled lubrication film of the problem.

**The vertical holding [force](../../../../../../force.md) is zero.** The geometry is invariant under a half-turn about the vertical axis. That operation reverses the horizontal angular [velocity](../../../../../../velocity.md) but leaves a vertical [force](../../../../../../force.md) component unchanged. Linearity would reverse that [force](../../../../../../force.md) component too, forcing it to vanish. Equivalently, the induced [pressure](../../../../../../pressure.md) has the first azimuthal harmonic, whose vertical-force integral over azimuth is zero. The horizontal holding [force](../../../../../../force.md) is the negative of the fluid's horizontal [force](../../../../../../force.md) on the body.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
