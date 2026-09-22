<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the plug-like [extensional viscosity](../../../../../../extensional-viscosity.md) approximation, [incompressibility](../../../../../../incompressible-flow.md) gives $w_z=-u_x$. Symmetry about $z=0$ fixes $w=-zu_x$. Remove the reference hydrostatic stress of the middle fluid, and write $S$ for its leading vertical normal stress. Vertical traction balance at the upper surface gives

$$
S=-\Delta\rho gh+\sigma_{zz}^+.
$$

The middle fluid's horizontal normal stress exceeds $S$ by $4\mu u_x$: the horizontal strain is $u_x$ and the vertical strain is $-u_x$. Hence

$$
\sigma_{xx}^{\mathrm{middle}}=S+4\mu u_x.
$$

At a slightly inclined upper interface, tangential traction continuity gives, to the order retained in the small-outer-viscosity extensional approximation,

$$
\sigma_{xz}^{\mathrm{middle}}(h)=\sigma_{xz}^++4\mu h_xu_x.
$$

The slope term is needed even though the interface is nearly horizontal: dropping it would miss the derivative of $h$ in the extensional resultant. Terms involving the outer deviatoric normal-stress difference times the slope are smaller in this approximation. Integrating horizontal force balance over the symmetric layer, or over its upper half, now gives

$$
0=h\partial_x(S+4\mu u_x)+\sigma_{xz}^{\mathrm{middle}}(h).
$$

Substitution yields the **extensional-flow equation**

$$
\boxed{4\mu\partial_x(hu_x)=h\partial_x(\Delta\rho gh-\sigma_{zz}^+)-\sigma_{xz}^+.}
$$

The full layer thickness is $2h$, so its [conservation of mass](../../../../../../mass-conservation.md) is $(2h)_t+(2hu)_x=0$, or

$$
\boxed{h_t+(hu)_x=0.}
$$

This explains the factor $4\mu$ in the extensional stress rather than the shear viscosity coefficient alone.

For a [Fourier mode](../../../../../../fourier-mode.md) of wave number $k>0$, set $h=h_0+\eta e^{ikx-st}$ and $u=\widehat u e^{ikx-st}$. Neglect $\sigma_{zz}^+$ as stipulated. The [Fourier traction map for a viscous half-space](../../../../../../fourier-traction-map-for-a-viscous-half-space.md), with outer [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\lambda\mu$, gives $\sigma_{xz}^+=-2\lambda\mu k\widehat u e^{ikx-st}$. The two linear equations are

$$
-4\mu h_0k^2\widehat u=ik\Delta\rho gh_0\eta+2\lambda\mu k\widehat u,
\qquad -s\eta+ikh_0\widehat u=0.
$$

Eliminating $\widehat u$ proves the **positive decay rate** for [relaxation of a symmetric viscous layer](../../../../../../relaxation-of-a-symmetric-viscous-layer.md):

$$
\boxed{s=\frac{\Delta\rho gh_0}{2\mu}\frac\kappa{\lambda+2\kappa},\qquad\kappa=kh_0.}
$$

When $\lambda\ll\kappa$, inner longitudinal extension dominates the [viscous dissipation](../../../../../../viscous-dissipation.md), and $s\sim\Delta\rho gh_0/(4\mu)$. When $\kappa\ll\lambda$ while the plug approximation remains valid, tangential motion of the semi-infinite outer fluids supplies the main resistance, and $s\sim\Delta\rho gh_0\kappa/(2\lambda\mu)$. The PDF's second inequality is $\kappa\ll\lambda$; the TeX converts it incorrectly to $\kappa\ll1$. At much larger outer viscosity the plug assumption fails, as the next calculation shows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
