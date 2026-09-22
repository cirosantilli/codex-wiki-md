<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Applying the stated long-wave expression formally in the intended high-viscosity regime, the numerator is dominated by $2\lambda\kappa^2/3$ and the displayed denominator by $\lambda$. It gives

$$
\boxed{s\sim\frac{\Delta\rho gh_0}{3\mu}\kappa^2.}
$$

The mechanism is inner transverse shear: the outer fluids almost immobilize the interfaces tangentially, so the middle layer has a pressure-driven parabolic velocity instead of the plug-like extensional velocity of part (b). Indeed, with nearly stationary faces at $z=\pm h$, its integrated flux is $-2h^3p_x/(3\mu)$. With $p_x=\Delta\rho gh_x$, [conservation of mass](../../../../../../mass-conservation.md) gives precisely the displayed decay rate. The leading [viscous dissipation](../../../../../../viscous-dissipation.md) is then in the middle layer, even though its neighbours have much greater [dynamic viscosity](../../../../../../dynamic-viscosity.md).

There is a nonuniformity in taking this conclusion literally for every $\lambda\gg\kappa^{-1}$. A long-wave remainder written for fixed $\lambda$ cannot be assumed uniform as $\lambda$ diverges. Here this matters physically because sufficiently viscous outer fluids also resist normal interface motion. The distinction can be resolved directly, without an unspecified remainder, from the [Stokes equation](../../../../../../stokes-equation.md). For a symmetric thickness mode, the middle vertical velocity has the form

$$
w(z)=A\sinh(kz)+B(kz)\cosh(kz),\qquad u=\frac i{k}w_z.
$$

It is odd in $z$, and the middle horizontal velocity is even. At $z=h_0$, the exact outer traction map is $\sigma_{xz}^+=-2\lambda\mu k u$ and $\sigma_{zz}^+=-2\lambda\mu k w$. Tangential continuity and the normal hydrostatic jump therefore give

$$
w_{zz}+k^2w=-2\lambda k w_z,\qquad
-\frac\mu{k^2}w_{zzz}+3\mu w_z+2\lambda\mu k w=-\Delta\rho g\eta.
$$

The latter uses $p=\mu(w_{zzz}-k^2w_z)/k^2$, obtained from horizontal force balance. The kinematic condition is $w(h_0)=-s\eta$. Writing $S=\sinh\kappa$ and $C=\cosh\kappa$, tangential continuity fixes

$$
A(S+\lambda C)+B[S+\kappa C+\lambda(C+\kappa S)]=0.
$$

Eliminating $A,B$ in the remaining two equations gives the **exact symmetric-layer rate**

$$
s=\frac{\Delta\rho gh_0}{2\mu\kappa}
\frac{S^2+\lambda(SC-\kappa)}{\lambda\cosh(2\kappa)+(SC+\kappa)+\lambda^2(SC-\kappa)}.
$$

For $\kappa\ll1$ and $\lambda\kappa\gg1$, this proves the [uniform high-viscosity limit of viscous-layer relaxation](../../../../../../uniform-high-viscosity-limit-of-viscous-layer-relaxation.md)

$$
\boxed{s\sim\frac{\Delta\rho gh_0}{2\mu}
\frac{(2/3)\kappa^2}{1+(2/3)\lambda\kappa^3}.}
$$

Thus the intended inner-shear answer is valid in the distinguished range $\kappa^{-1}\ll\lambda\ll\kappa^{-3}$. If $\lambda\kappa^3\gg1$, the main resistance is instead outer normal motion and

$$
s\sim\frac{\Delta\rho g}{2\lambda\mu k}.
$$

Both ranges satisfy the printed $\lambda\gg\kappa^{-1}\gg1$. For example $\lambda=\kappa^{-4}$ lies in the latter range and has $s\sim[\Delta\rho gh_0/(2\mu)]\kappa^3$, rather than a rate proportional to $\kappa^2$. The exact denominator contains a $\lambda^2\kappa^3$ contribution hidden by a fixed-parameter remainder. **The inner-shear limit is the intended result, but an additional upper restriction on $\lambda$ is needed to make it a uniform conclusion.**

## ↑ Ancestors (11)

1. [C](../c.md)
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
