<h1 id="3/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a rough boundary, integrate the similarity shear from the [roughness length](../../../../../../../roughness-length.md). A usual moderate-stability closure is

$$
\phi_m(\zeta)=1+c_s\zeta\quad(\zeta\geq0),\qquad \phi_m(\zeta)=(1-c_u\zeta)^{-1/4}\quad(\zeta\leq0),
$$

with positive dimensionless coefficients. These are empirical closures, not quantities determined by similarity alone. An often-used choice is $c_s=5,c_u=16$. The unstable quarter-power relation is tested over approximately $-1\lesssim z/\ell_O\lesssim-0.01$ in [Dyer's flux-gradient study](https://rmets.onlinelibrary.wiley.com/doi/10.1002/qj.49709641012); the stable coefficient convention is recorded in [the surface-flux formulation](https://journals.ametsoc.org/view/journals/apme/36/10/1520-0450_1997_036_1416_iosfci_2.0.co_2.xml). Near neutrality one takes their smooth limits.

For moderate stable conditions, integration gives

$$
\boxed{U(z)=\frac{u_*}{\kappa}\left[\log\frac z{z_0}+c_s\frac{z-z_0}{\ell_O}\right].}
$$

For the unstable closure set $x(\zeta)=(1-c_u\zeta)^{1/4}$ and define

$$
\psi_m(\zeta)=2\log\frac{1+x}{2}+\log\frac{1+x^2}{2}-2\arctan x+\frac\pi2.
$$

Then $1-\zeta\psi_m'(\zeta)=\phi_m(\zeta)$ and

$$
\boxed{U(z)=\frac{u_*}{\kappa}\left[\log\frac z{z_0}-\psi_m(z/\ell_O)+\psi_m(z_0/\ell_O)\right].}
$$

For weak unstable departure, $|c_u z/\ell_O|\ll1$, this reduces to the stable-form expression with $c_s$ replaced by $c_u/4$ and a negative $\ell_O$. The full quarter-power expression is useful for moderately unstable conditions with $|z/\ell_O|$ of order one; it must not be extrapolated automatically to the distinct asymptotic free-convection regime. The stable linear expression similarly describes a continuously turbulent surface layer, rather than guaranteeing validity after strong stratification destroys the constant-flux state. Both profiles require $z_0\ll z\ll\delta_\tau$ and approximately uniform fluxes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 79](../../../../paper-79-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
