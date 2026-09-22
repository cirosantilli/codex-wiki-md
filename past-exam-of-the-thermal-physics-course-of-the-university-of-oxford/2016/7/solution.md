<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Let the gas have a small bulk [velocity](../../../velocity.md) $u_x(y)$, an approximately isotropic local thermal velocity distribution, and a [mean free path](../../../mean-free-path.md) $\lambda$ short compared with the flow-gradient scale. A molecule transports the mean streamwise [momentum](../../../momentum-split.md) acquired near its previous collision. To first order, its nonequilibrium momentum relative to the destination layer is approximately $-m\tau_c v_y\,du_x/dy$. The resulting transverse [momentum flux](../../../momentum-flux.md) is

$$
\Pi_{xy}\simeq-nm\tau_c\langle v_y^2\rangle\frac{du_x}{dy}.
$$

Thus the [dynamic viscosity](../../../dynamic-viscosity-split.md) is $\eta\simeq\rho\tau_c\langle v_y^2\rangle$. With isotropy, a representative collision time $\tau_c\sim\lambda/\langle v\rangle$, and a chosen thermal speed average, this has the form

$$
\boxed{\eta=K\rho\langle v\rangle\lambda.}
$$

The dimensionless $K$ depends on how speeds and collision times are averaged; a simple one-speed estimate gives $K=1/3$. Assumptions include dilute binary collisions, a locally equilibrated distribution, weak shear, and negligible boundary slip. The [kinetic theory](../../../kinetic-theory-split.md) identity $p=\rho\langle v^2\rangle/3$ then gives

$$
\frac p\eta=\frac{\langle v^2\rangle}{3K\langle v\rangle^2}\frac{\langle v\rangle}{\lambda}.
$$

For the [Maxwell speed distribution](../../../maxwell-speed-distribution.md), $\langle v^2\rangle/\langle v\rangle^2=3\pi/8$, so

$$
\boxed{\frac p\eta=\frac\pi{8K}\,\nu_{\rm coll},\qquad \nu_{\rm coll}\simeq\frac{\langle v\rangle}{\lambda}.}
$$

This explains both the units of inverse time and the relation to molecular collision frequency, up to the averaging convention.

In the cylinder apparatus, distinguish the vector mean molecular [velocity](../../../velocity.md), $\langle\mathbf v\rangle=\mathbf u$, from the mean thermal speed $\langle|\mathbf v-\mathbf u|\rangle$. For a slow nearly isothermal [Couette flow](../../../couette-flow.md), the thermal speed is approximately position-independent, whereas the bulk mean is azimuthal and changes from the local rotating-wall speed to zero at the fixed wall. In the side gap, with $y$ measured radially from the inner wall,

$$
u_\varphi(y)\simeq\omega R\left(1-\frac yh\right),\qquad 0\le y\le h.
$$

Across either end gap, at cylindrical radius $s$, the corresponding profile is $u_\varphi(s,z)\simeq\omega s(1-z/h)$, with $z$ measured away from the moving end face. The [no-slip boundary condition](../../../no-slip-boundary-condition.md) and small $h/R,h/H$ underlie these linear profiles.

The side-wall [shear stress](../../../shear-stress.md) has magnitude $\eta\omega R/h$, producing resisting [torque](../../../torque.md) $2\pi\eta\omega R^3H/h$. **The original diagram also has a gap at both circular end faces.** At either face, the stress is $\eta\omega s/h$ and its ring contribution is

$$
d\tau_{\rm end}=s\left(\frac{\eta\omega s}{h}\right)2\pi s\,ds,
\qquad \tau_{\rm end}=\frac{\pi\eta\omega R^4}{2h}.
$$

Adding the side and both ends gives the [end-face torque in narrow-gap cylindrical viscometry](../../../end-face-torque-in-narrow-gap-cylindrical-viscometry.md):

$$
\boxed{\tau=C\eta\omega,\qquad C=\frac\pi h\left(2R^3H+R^4\right).}
$$

The motor supplies the opposite of this viscous resisting [torque](../../../torque.md). Corner flow and the small axle area are neglected. Retaining only the cylindrical wall would omit the $\pi R^4/h$ term shown by the actual closed-ended geometry.

For hard-sphere Ar atoms of collision diameter $d_{\rm Ar}$, $\lambda=1/(\sqrt2n\pi d_{\rm Ar}^2)$ and $\rho=nm_{\rm Ar}$. Therefore

$$
d_{\rm Ar}=\left[\frac{K m_{\rm Ar}\langle v\rangle}{\sqrt2\pi\eta}\right]^{1/2},\qquad
\langle v\rangle=\sqrt{\frac{8k_BT}{\pi m_{\rm Ar}}}.
$$

Using $m_{\rm Ar}=40m_u$, $T=273.15\,\mathrm K$ and the simple estimate $K=1/3$ gives

$$
\boxed{\langle v\rangle\simeq380\,\mathrm{m\,s^{-1}},\qquad d_{\rm Ar}\simeq3.0\times10^{-10}\,\mathrm m.}
$$

This is a kinetic estimate with a model-dependent numerical prefactor, rather than a precise atomic size measurement. Since the density cancels and the hard-sphere collision diameter is taken constant, the prediction is $\eta\propto\sqrt T$. The collision cross-section of a real atom can vary with speed, so its exact temperature dependence need not follow this power law.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2016](../../2016-split.md)
3. [Past exam of the thermal physics course of the University of Oxford](../../split.md)
4. [Thermal physics course of the University of Oxford](../../../thermal-physics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
