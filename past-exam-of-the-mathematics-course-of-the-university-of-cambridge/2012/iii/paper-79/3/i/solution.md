<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define the positive total shear stress by $\tau=\rho[\nu U_z-\overline{u'w'}]$, so the physical wall traction on the fluid opposes the positive flow. The steady mean momentum equation gives

$$
0=-P_x+\tau_z,\qquad\boxed{\tau(z)=\tau_S+P_xz.}
$$

For a driving pressure gradient $P_x<0$, the stress decreases upward. It is approximately constant while

$$
\boxed{z\ll\delta_\tau=\tau_S/|P_x|,\qquad u_*=\sqrt{\tau_S/\rho}.}
$$

An outer boundary-layer height can impose a stricter limit. In the turbulent region outside the viscous or roughness sublayer, the only local neutral scales are $u_*$ and $z$, so $U_z=C u_*/z$. Conventionally write $C=1/\kappa$, where $\kappa$ is the von Kármán constant. Equivalently, a mixing length $\ell=\kappa z$ and stress closure $u_*^2=\ell^2U_z^2$ give the same result. Integration yields the [law of the wall](../../../../../../law-of-the-wall.md)

$$
\boxed{U(z)=\frac{u_*}{\kappa}\log\frac z{z_0}.}
$$

The [roughness length](../../../../../../roughness-length.md) $z_0$ is an extrapolation scale, not a statement that the logarithm is valid at the actual solid surface. For a smooth boundary, the viscous inner scales are $z^+=zu_*/\nu$, $U^+=U/u_*$. The viscous sublayer has $U^+\simeq z^+$; farther out $U^+=\kappa^{-1}\log z^++C_s$, corresponding to $z_0=(\nu/u_*)e^{-\kappa C_s}$. For a fully rough boundary, $z_0$ is proportional to a geometric roughness height and viscosity no longer determines the leading profile. The logarithmic region still needs roughness height $\ll z\ll\delta_\tau$.

In local equilibrium, production of [turbulent kinetic energy](../../../../../../turbulent-kinetic-energy.md) by the shear is $P=-\overline{u'w'}U_z\simeq u_*^2U_z$. Neglecting its transport relative to production and [viscous dissipation](../../../../../../viscous-dissipation.md),

$$
\boxed{\epsilon\simeq\frac{u_*^3}{\kappa z}.}
$$

Dimensional similarity alone gives $\epsilon\propto u_*^3/z$; the displayed coefficient additionally uses the local energy balance and the logarithmic shear.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
