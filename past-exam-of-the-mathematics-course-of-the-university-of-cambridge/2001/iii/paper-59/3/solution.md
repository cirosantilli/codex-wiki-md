<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The real [scalar field](../../../../../scalar-field.md) has [canonical momentum](../../../../../canonical-momentum.md) $\pi=\dot\phi$. Its [Legendre transform](../../../../../convex-conjugate.md) gives

$$
\boxed{H=\int d^3x\left[\frac12\pi^2+\frac12(\nabla\phi)^2+\frac12m^2\phi^2+\frac{\lambda}{4!}\phi^4\right].}
$$

The first three terms constitute $H_0$, the free massive [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md). The remaining term is $H_I=\lambda\int\phi^4d^3x/4!=-\int\mathcal L_I d^3x$. This sign is a consequence of having no time derivatives in the interaction: the [canonical momentum](../../../../../canonical-momentum.md) is unchanged, while the interaction enters the [Hamiltonian density](../../../../../hamiltonian-density.md) with the opposite sign to the [Lagrangian density](../../../../../lagrangian-density.md).

In the [interaction picture](../../../../../interaction-picture.md), operators evolve with $H_0$ and states evolve with $H_I(t)$ constructed from the free interaction-picture field. Their evolution operator satisfies

$$
i\partial_tU_I(t,t_0)=H_I(t)U_I(t,t_0),\qquad U_I(t_0,t_0)=I.
$$

Integrating once gives $U_I=I-i\int_{t_0}^tH_I(t_1)U_I(t_1,t_0)dt_1$. Repeated substitution orders the integrations as $t\geq t_1\geq\cdots\geq t_n\geq t_0$. Replacing the ordered simplex by the full integration cube introduces $1/n!$ and a [time-ordered product](../../../../../time-ordered-product.md), which proves the [Dyson series](../../../../../dyson-series.md)

$$
U_I(t,t_0)=\sum_{n=0}^\infty\frac{(-i)^n}{n!}\int_{t_0}^t dt_1\cdots dt_n\,
\mathrm T\{H_I(t_1)\cdots H_I(t_n)\}.
$$

Taking the asymptotic limits with the usual adiabatic or regulated scattering prescription yields

$$
\boxed{S=\mathrm T\exp\left[-i\int_{-\infty}^{\infty}H_I(t)dt\right]
=\mathrm T\exp\left[i\int d^4x\,\mathcal L_I(\phi_I(x))\right].}
$$

The field in this expression is the free field evolving in the [interaction picture](../../../../../interaction-picture.md), not an independently prescribed classical field. For quantum fields the expansion is a regulated perturbation series; the time-ordering symbol cannot be dropped because the operators at different times need not commute.

Use relativistically normalized two-particle states $|p_1,p_2\rangle=a^\dagger(p_1)a^\dagger(p_2)|0\rangle$, with $\langle p|q\rangle=(2\pi)^3 2E_p\delta^3(\mathbf p-\mathbf q)$. The connected first-order scattering contribution is

$$
\langle p_3,p_4|(S-I)|p_1,p_2\rangle_{\rm conn}
=-\frac{i\lambda}{4!}\int d^4x\,
\langle p_3,p_4|:\!\phi_I(x)^4\!:|p_1,p_2\rangle.
$$

Here the connected [S-matrix](../../../../../s-matrix.md) uses a normalized vacuum and physical external one-particle states. At this order, [normal ordering](../../../../../normal-ordering.md) the vertex separates the four-external-leg contribution from vacuum and tadpole pieces; those disconnected or external-mass contributions are not the two-to-two scattering amplitude.

Two fields annihilate the incoming particles and two create the outgoing ones. There are $\binom42$ choices of the annihilating fields, two assignments of the incoming [momenta](../../../../../momentum.md) and two assignments of the outgoing [momenta](../../../../../momentum.md). Hence the total factor is $\binom42\,2!\,2!=4!$, the [external-leg factorial cancellation at a quartic scalar vertex](../../../../../external-leg-factorial-cancellation-at-a-quartic-scalar-vertex.md). Each attachment contributes its plane-wave factor, so

$$
\langle p_3,p_4|:\!\phi_I(x)^4\!:|p_1,p_2\rangle_{\rm conn}
=4!e^{i(p_3+p_4-p_1-p_2)\cdot x}.
$$

The spacetime integral is the [four-momentum conservation](../../../../../four-momentum-conservation.md) delta function, giving

$$
\boxed{\langle p_3,p_4|(S-I)|p_1,p_2\rangle_{\rm conn}
=i(2\pi)^4\delta^4(p_3+p_4-p_1-p_2)T,\qquad T=-\lambda+O(\lambda^2).}
$$

In particular, the tree [scattering amplitude](../../../../../scattering-amplitude.md) is independent of angle.

For completeness, derive the [relativistic two-body phase space](../../../../../relativistic-two-body-phase-space.md) in the centre-of-mass frame. Write $\sqrt s=2E_*$, $p_*^2=E_*^2-m^2$. The spatial delta function sets the two final [momenta](../../../../../momentum.md) opposite, and the [energy](../../../../../energy.md) delta function is $\delta(\sqrt s-2\sqrt{p^2+m^2})$. Its radial Jacobian is $E_*/(2p_*)$. Thus

$$
d\Phi_2=\frac1{16\pi^2}\frac{p^2dp}{E_p^2}\delta(\sqrt s-2E_p)d\Omega
=\frac{p_*}{16\pi^2\sqrt s}\,d\Omega.
$$

The [invariant flux factor](../../../../../invariant-flux-factor.md) is $\mathcal F=4p_*\sqrt s$ for equal initial masses. Using $d\sigma=|T|^2d\Phi_2/\mathcal F$, the labeled angular density is $\lambda^2/(64\pi^2s)$. The outgoing quanta belong to one real [scalar field](../../../../../scalar-field.md), so they are identical. A full-sphere integration counts each event twice and requires the [identical final-state symmetry factor](../../../../../identical-particle-factor-in-a-final-state-phase-space-integral.md) $1/2!$. Consequently

$$
\boxed{\sigma=\frac12\int_{S^2}\frac{\lambda^2}{64\pi^2s}d\Omega
=\frac{\lambda^2}{32\pi s}+O(\lambda^3),\qquad s>4m^2.}
$$

Equivalently one may integrate the labeled density over a hemisphere representing each event once. The final-state factor is separate from the vertex factorial: applying it at the vertex instead would give the wrong [elastic scattering from a quartic scalar contact interaction](../../../../../elastic-scattering-from-a-quartic-scalar-contact-interaction.md) cross-section.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
