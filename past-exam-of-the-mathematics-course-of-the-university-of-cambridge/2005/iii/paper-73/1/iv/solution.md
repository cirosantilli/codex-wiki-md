<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Estimate characteristic bulk terms. Put $\epsilon=H/r\ll1$ and assume smooth radial variation on scale $r$, secular evolution, and $\alpha\lesssim1$. Vertical support gives $c_s^2\sim p/\rho\sim\Omega^2H^2$, while the [alpha disk](../../../../../../alpha-disk.md) prescription and slow accretion imply

$$
\nu\sim\alpha\Omega H^2,\qquad u_r\sim\frac\nu r,\qquad u_z\sim\frac Hr u_r.
$$

These velocity estimates follow from the viscous radial evolution scale and [mass conservation](../../../../../../mass-conservation.md). They are estimates for a slowly evolving thin disc, not a claim that geometric thinness excludes independently forced rapid vertical motion.

For vertical balance, the exact central force expands as

$$
\frac{GMz}{(r^2+z^2)^{3/2}}=\Omega_K^2z\left[1-\frac32\frac{z^2}{r^2}+O\!\left(\frac{z^4}{r^4}\right)\right].
$$

At $z\sim H$, the neglected correction has magnitude $\rho\Omega^2H\epsilon^2$, compared with the retained force $\rho\Omega^2H$. Radial [pressure](../../../../../../pressure.md) support similarly changes the rotation from its Keplerian value by

$$
\frac{\delta\Omega^2}{\Omega_K^2}\sim\frac{c_s^2}{r^2\Omega_K^2}=O(\epsilon^2).
$$

Vertical meridional inertia scales as $u_r u_z/r$ or $u_z^2/H$, both $O(\alpha^2\epsilon^4\Omega^2H)$. Meridional viscous accelerations can scale as $\nu u_z/H^2$ or $\nu u_r/(rH)$, both $O(\alpha^2\epsilon^2\Omega^2H)$. Thus the gravity correction and possible viscous correction give

$$
\boxed{\frac{\text{neglected vertical-force terms}}{\rho\Omega^2H}=O(\epsilon^2).}
$$

Some omitted terms are smaller than this leading order.

For the heating equation, the retained dissipation is $q_0^+\sim\rho\nu\Omega^2\sim\alpha p\Omega$. Radial [pressure](../../../../../../pressure.md) support and the finite-height correction change the dominant shear by a relative $O(\epsilon^2)$. Smooth vertical variation of the rotation gives $\partial_z(r\Omega)=O(\epsilon\Omega)$, whose additional squared shear contributes $O(\epsilon^2q_0^+)$. Meridional shear of order $u_r/H$ gives an additional relative $O(\alpha^2\epsilon^2)$ contribution.

Thermal [advection](../../../../../../advection.md) and compressional work are of order $\rho u_r c_s^2/r$ and $p u_r/r$, respectively. Relative to $\alpha p\Omega$ they are $O(\epsilon^2)$. Thermal storage on the viscous evolution timescale $t_\nu\sim r^2/\nu$ has the same order, since $p/t_\nu\sim\alpha p\Omega\epsilon^2$. For [radiative diffusion](../../../../../../radiative-diffusion.md) with the same local diffusivity in different directions, smooth gradients give $F_r/F_z\sim H/r$, so

$$
\frac{r^{-1}\partial_r(rF_r)}{\partial_zF_z}\sim\frac{F_r/r}{F_z/H}=O(\epsilon^2).
$$

Consequently

$$
\boxed{\frac{\text{neglected local-energy terms}}{(9/4)\alpha\Omega p}=O\!\left((H/r)^2\right).}
$$

This is the [thin-accretion-disk truncation error](../../../../../../thin-accretion-disk-truncation-error.md) for the secular, radially smooth approximation. Neglect of disc [self-gravity](../../../../../../self-gravity.md) and [radiation pressure](../../../../../../radiation-pressure.md), optical thickness, the opacity model and the idealized zero surface boundary have their own validity conditions; their errors do not become small solely because $H/r$ does. Near a sharp radial [boundary layer](../../../../../../boundary-layer.md) or during thermal evolution on the heating timescale, the above estimates need not apply.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
