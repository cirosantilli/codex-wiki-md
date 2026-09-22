<h1 id="38a/solution">Solution</h1>

↑ **Parent:** [38A](../38a.md)

Start from $\rho(\partial_tu+u\cdot\nabla u)=-\nabla p-\rho ge_z$, $\partial_t\rho+u\cdot\nabla\rho=0$, and $\nabla\cdot u=0$. The stationary background obeys $p_0'=-g\rho_0$. Linearize in small perturbations and use the [Boussinesq approximation](../../../../../boussinesq-approximation.md): replace the density by a reference value $\rho_*$ in inertia but retain the density perturbation in the buoyancy force. With $\pi=p'/\rho_*$ and $b=-g\rho'/\rho_*$,

$$
u_t=-\nabla\pi+be_z,\qquad b_t+N^2w=0,\qquad\nabla\cdot u=0,\qquad
\boxed{N^2=-\frac g{\rho_*}\frac{d\rho_0}{dz}>0.}
$$

This is the [Brunt–Väisälä frequency](../../../../../buoyancy-frequency.md). Its assumed constancy requires a locally uniform stable density gradient in this approximation; rotation and viscosity are neglected.

For a [plane wave](../../../../../plane-wave.md) with wavevector $K=(k,\ell,m)$, project the momentum equation onto the space perpendicular to $K$ to eliminate pressure. Its vertical component is $-i\omega w=b[1-m^2/|K|^2]$, while $-i\omega b+N^2w=0$. Eliminating $b$ yields

$$
\boxed{\omega^2=\frac{N^2(k^2+\ell^2)}{k^2+\ell^2+m^2}.}
$$

For $0<\omega<N$, a small oscillating body radiates upward and downward conical [internal gravity wave](../../../../../internal-wave.md) beams. In a vertical section the beams make a St Andrew's cross, with angle $\alpha$ to the horizontal satisfying $\sin\alpha=\omega/N$. Indeed the [group velocity](../../../../../group-velocity.md) is perpendicular to the wavevector and has ratio of vertical to horizontal magnitudes $\sqrt{k^2+\ell^2}/|m|$. Thus wave energy follows the cones, rather than the direction normal to a fixed-radius spherical wavefront. There are no such propagating beams for $\omega>N$.

For the shear-flow calculation choose the positive intrinsic-frequency branch and $k_0>0$, conditions needed for the printed critical-level formula. The slowly varying local dispersion relation is

$$
\Omega=kU(z)+\widehat\omega,\qquad\widehat\omega=\frac{Nk}{\sqrt{k^2+m^2}}.
$$

Stationarity and horizontal homogeneity conserve $\Omega$ and $k=k_0$. The [Hamiltonian ray equations for a local dispersion relation](../../../../../hamiltonian-ray-equations-for-a-local-dispersion-relation.md) give

$$
\dot z=\partial_m\Omega=-\frac{Nk_0m}{(k_0^2+m^2)^{3/2}},\qquad\dot m=-\partial_z\Omega=-k_0U'(z)<0.
$$

Thus $m_0<0$ stays negative and the ray propagates upward. Conservation of frequency gives

$$
\widehat\omega(z)=\frac{Nk_0}{\sqrt{k_0^2+m_0^2}}-k_0[U(z)-U(0)].
$$

If the shear reaches the required velocity difference, its first zero is the [critical level of an internal gravity wave](../../../../../critical-level-of-an-internal-gravity-wave.md),

$$
\boxed{U(z_c)-U(0)=\frac N{\sqrt{k_0^2+m_0^2}}.}
$$

As $z\uparrow z_c$, the intrinsic frequency tends to zero, $m\to-\infty$, the vertical wavelength tends to zero and the vertical [group velocity](../../../../../group-velocity.md) tends to zero. The ideal ray cannot cross this level. For finite $U'_c>0$, $\dot z\sim k_0(U'_c)^2(z_c-z)^2/N$, so it approaches the level only asymptotically in time. The disturbance develops short scales; even weak viscosity can then absorb it, and nonlinear effects can invalidate the small-amplitude approximation.

**The printed sign and existence hypotheses are incomplete.** On the positive-frequency branch, $k_0<0$ instead gives $\dot m>0$ and eventually a turning point when the intrinsic frequency reaches $N$. As a concrete counterexample to the stated universal height bound, take $N=1$, $k_0=-1$, $m_0=-3$, and $U(z)=\varepsilon z$ with any small $\varepsilon>0$. At the printed height $z_c=1/(\varepsilon\sqrt{10})$, the intrinsic frequency is $2/\sqrt{10}<1$ and $m=-\sqrt{3/2}<0$, so the vertical [group velocity](../../../../../group-velocity.md) is still positive and the ray crosses that height. Also, $U'>0$ alone does not ensure that the displayed velocity difference is ever reached; an increasing bounded $U$ may have no finite critical level. The qualified derivation above gives the intended positive-$k_0$ result whenever that level exists.

## ↑ Ancestors (10)

1. [38A](../38a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
