<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let primes denote radial derivatives of the equilibrium and put $\Delta u=u'+2u/r$. The linearized continuity, adiabatic pressure and [Poisson equation](../../../../../poisson-equation.md) are

$$
\partial_t\delta\rho=-\frac1{r^2}\partial_r(r^2\rho u)=-\rho\Delta u-\rho'u,
\qquad \partial_t\delta p=-u p'-\gamma p\Delta u,
\qquad \partial_r(r^2\partial_r\delta\Phi)=4\pi G r^2\delta\rho.
$$

Take the time derivative of the [Poisson equation](../../../../../poisson-equation.md) and substitute continuity. Integration in radius gives

$$
r^2\partial_r\partial_t\delta\Phi=-4\pi G r^2\rho u+C(t).
$$

Centre regularity excludes a changing point mass at the origin, so $C(t)=0$ and

$$
\boxed{\partial_r\partial_t\delta\Phi=-4\pi G\rho u.}
$$

The perturbed [self-gravity](../../../../../self-gravity.md) must be retained; this calculation does not make the [Cowling approximation](../../../../../cowling-approximation.md).

The radial linear momentum equation is $\rho\partial_tu=-\partial_r\delta p-\delta\rho\Phi'-\rho\partial_r\delta\Phi$. Differentiate it in time and use the preceding equations:

$$
\rho\partial_t^2u=\partial_r(\gamma p\Delta u)+\partial_r(up')+(\rho\Delta u+\rho'u)\Phi'+4\pi G\rho^2u.
$$

The equilibrium has $p'=-\rho\Phi'$ and $\Phi''+2\Phi'/r=4\pi G\rho$. The remaining terms simplify as

$$
\partial_r(up')+(\rho\Delta u+\rho'u)\Phi'+4\pi G\rho^2u
=-\frac{2up'}r+\rho u(4\pi G\rho-\Phi'')=-\frac{4up'}r.
$$

Consequently the radial [stellar oscillation](../../../../../stellar-oscillation.md) equation is

$$
\boxed{\rho\partial_t^2u=\partial_r(\gamma p\Delta u)-\frac{4u}r p'.}
$$

The derivative acts on the full variable coefficient $\gamma(r)p(r)$; discarding $\gamma'$ would change the result.

For $u=r\xi(r)e^{-i\omega t}$, $\Delta u=(3\xi+r\xi')e^{-i\omega t}$. Substitute and multiply by $-r^3$. Combining the two terms proportional to $\xi'$ into a total derivative gives the [radial stellar pulsation equation](../../../../../radial-stellar-pulsation-equation.md),

$$
\boxed{\omega^2\rho r^4\xi=-\frac{d}{dr}\left(\gamma p r^4\xi'\right)+r^3\frac{d}{dr}\bigl((4-3\gamma)p\bigr)\xi.}
$$

Set $P=\gamma p r^4$, $W=\rho r^4$ and $Q=r^3[(4-3\gamma)p]'$. The [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) is

$$
L\xi=\frac1W\bigl[-(P\xi')'+Q\xi\bigr],\qquad
\langle\eta,\xi\rangle_W=\int_0^{R_s}W\eta^*\xi\,dr.
$$

For regular physical perturbations, $\xi$ is finite at the centre and $P\xi'\to0$ at the free surface. For a nonzero-frequency mode the [fluid displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) is $u/(-i\omega)$, so vanishing [Lagrangian pressure perturbation](../../../../../lagrangian-pressure-perturbation.md) is equivalent to $\gamma p(3\xi+r\xi')\to0$. With $p(R_s)=0$ and finite $\xi$, this gives $P\xi'\to0$. Zero-frequency modes use the same displacement boundary condition directly. Assume bounded $\gamma$, positive $\rho,p,\gamma$ in the interior and the usual finite-energy endpoint domain. Integration by parts gives

$$
\langle\eta,L\xi\rangle_W-\langle L\eta,\xi\rangle_W
=\left[P(\eta'^*\xi-\eta^*\xi')\right]_0^{R_s}=0.
$$

Thus this physical [self-adjoint differential operator](../../../../../self-adjoint-differential-operator.md) has real [eigenvalues](../../../../../eigenvalue.md) $\omega^2$. The endpoint domain is essential: the fact that $p$ vanishes does not by itself allow arbitrary singular trial functions. The regular free-surface realization of the [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) is the one used here.

The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) gives the fundamental squared frequency as the infimum of the [weighted stellar pulsation Rayleigh quotient](../../../../../weighted-stellar-pulsation-rayleigh-quotient.md),

$$
\boxed{\omega_0^2=\inf_{\xi\ne0}\frac{\displaystyle\int_0^{R_s}\left[\gamma p r^4|\xi'|^2+r^3\bigl((4-3\gamma)p\bigr)'|\xi|^2\right]dr}{\displaystyle\int_0^{R_s}\rho r^4|\xi|^2dr}.}
$$

The infimum is over admissible finite-energy functions satisfying the physical endpoint conditions. If this quotient is nonnegative for every such function, all radial frequencies are real and there is no exponentially growing radial mode. A negative value for even one trial function proves a negative [eigenvalue](../../../../../eigenvalue.md) and an exponentially growing solution, because $\omega^2<0$. A zero lowest value is marginal and needs separate treatment of neutral motion.

Choose the homologous trial function $\xi=1$, which corresponds to radial velocity proportional to $r$. Its gradient contribution is zero, and

$$
\int_0^{R_s}r^3[(4-3\gamma)p]'dr
=\left[r^3(4-3\gamma)p\right]_0^{R_s}-3\int_0^{R_s}r^2p(4-3\gamma)dr
=-3\int_0^{R_s}r^2p(4-3\gamma)dr.
$$

The denominator $\int\rho r^4dr$ is positive. Hence

$$
\boxed{\int_0^{R_s}r^2p(4-3\gamma)dr>0\ \Longrightarrow\ \omega_0^2<0\ \Longrightarrow\ \text{radial instability}.}
$$

This [pressure-weighted radial instability criterion](../../../../../pressure-weighted-radial-instability-criterion.md) is sufficient, not necessary: another trial function can detect instability even if this one does not. For a constant [stellar adiabatic exponent](../../../../../stellar-adiabatic-exponent.md) it recovers instability below $4/3$. At constant $\gamma=4/3$, the homologous mode is neutral. For constant $\gamma>4/3$, $Q=(4-3\gamma)r^3p'>0$ in a normally stratified [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md), so the quotient is positive and the star is radially stable.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
