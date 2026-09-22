<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fully ionized hydrogen, the outward radiation force on a coupled proton-electron pair at radius $r$ is $\sigma_TL/(4\pi r^2c)$, while its inward gravitational force is approximately $GMm_p/r^2$. Equating them yields the [Eddington luminosity](../../../../../../eddington-luminosity.md),

$$
\boxed{L_{\rm Edd}=\frac{4\pi GMm_pc}{\sigma_T}.}
$$

This uses isotropic radiation, [Thomson scattering](../../../../../../thomson-scattering.md) and efficient momentum coupling between electrons and ions. Composition or other opacity sources alter the corresponding limit.

With radiative efficiency $\epsilon_r$, a rest-mass supply rate gives $L=\epsilon_r\dot M_{\rm in}c^2$. In the approximation that supplied mass is added to the hole, continuous accretion at the [Eddington luminosity](../../../../../../eddington-luminosity.md) gives

$$
\dot M\simeq\frac{L_{\rm Edd}}{\epsilon_rc^2}=\frac M{t_e},\qquad
\boxed{M(t)=M_0e^{t/t_e},\quad t_e\simeq\epsilon_r\frac{c\sigma_T}{4\pi Gm_p}\simeq4.5\times10^8\epsilon_r\,\mathrm{yr}.}
$$

Here $t$ is the elapsed time since seed formation. If the radiated rest mass is counted exactly, $\dot M=(1-\epsilon_r)\dot M_{\rm in}$ and the [Salpeter time](../../../../../../salpeter-time.md) becomes $t_e=\epsilon_r c\sigma_T/[(1-\epsilon_r)4\pi Gm_p]$. The displayed approximation in the question neglects this correction; retaining it lengthens the growth time.

The required growth factor is $10^7$, corresponding to $\ln(10^7)=16.12$ e-folds. With the supplied efficiency,

$$
\boxed{t_{\rm grow}\simeq45\,\mathrm{Myr}\times16.12\simeq725\,\mathrm{Myr}.}
$$

At $z=8$, the expansion is overwhelmingly matter-dominated. Using total $\Omega_{\rm mat}=0.25$ and $H_0=70\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$ gives

$$
t(z)\simeq\int_z^\infty\frac{dz'}{H_0\sqrt{\Omega_{\rm mat}}(1+z')^{5/2}}
=\frac{2}{3H_0\sqrt{\Omega_{\rm mat}}}(1+z)^{-3/2},
\qquad\boxed{t(z=8)\simeq690\,\mathrm{Myr}.}
$$

The baryon density is part of the total matter density, so it is not added to $\Omega_{\rm mat}$ in this age calculation. Dark-energy and radiation corrections are small for this estimate. Even starting at the earliest possible time, the approximate growth time exceeds the age, and a real stellar seed forms later. **A $30M_\odot$ seed cannot reach the stated mass through uninterrupted Eddington-limited growth with the stated efficiency.** Exactly retaining the radiated mass gives about $806\,\mathrm{Myr}$ and strengthens this conclusion. A heavier seed, lower radiative efficiency or super-Eddington episodes can relieve the time constraint; interruptions make it harder.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
