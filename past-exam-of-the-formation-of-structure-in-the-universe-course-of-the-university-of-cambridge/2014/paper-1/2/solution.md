<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Radial [epicyclic motion](../../../../epicyclic-motion.md).** At fixed [specific angular momentum](../../../../specific-angular-momentum.md), use $\Phi_{\rm eff}=\Phi+\ell^2/(2r^2)$ and $\ddot r=-\Phi_{\rm eff}'$. A [circular orbit](../../../../circular-orbit.md) at $r_c$ obeys $\Phi'(r_c)=\ell^2/r_c^3=r_c\Omega^2$. Expanding $r=r_c+\xi$ gives $\ddot\xi+\kappa^2\xi=0$, where

$$
\boxed{\kappa^2=\Phi''+\frac{3\ell^2}{r_c^4}
=4\Omega^2+2r_c\Omega\Omega'
=4\Omega^2\left(1+\frac{r_c\Omega'}{2\Omega}\right)}.
$$

For $\kappa^2>0$ the [radial epicyclic frequency](../../../../radial-epicyclic-frequency.md) describes [simple harmonic motion](../../../../simple-harmonic-motion.md). The angular correction follows from [conservation of angular momentum](../../../../conservation-of-angular-momentum.md), $\dot\phi\simeq\Omega(1-2\xi/r_c)$, and describes an [epicyclic motion](../../../../epicyclic-motion.md) around the guiding [circular orbit](../../../../circular-orbit.md).

**Stabilizing terms.** In the given local fluid [dispersion relation](../../../../dispersion-relation-split.md), $\kappa^2$ is rotational support, important at long [wavelength](../../../../wavelength.md); $a_0^2k^2$ is random-motion or [pressure](../../../../pressure-split.md) support, important at short [wavelength](../../../../wavelength.md). The term $-2\pi G\Sigma|k|$ is destabilizing [self-gravity](../../../../self-gravity.md). Although the wording refers to stellar dispersion, this algebra uses the supplied fluid approximation; a collisionless stellar treatment has a reduction factor and a different numerical normalization.[Abstract and Sections II–V: collisionless stability threshold and random-motion support](../../../../on-the-gravitational-stability-of-a-disk-of-stars-by-alar-toomre.md)

**Axisymmetric threshold.** For $n=0$, set $q=|k|\geq0$. Completing the square gives

$$
\omega^2=a_0^2(q-q_*)^2+\kappa^2(1-Q^{-2}),
\qquad q_*=\frac{\pi G\Sigma}{a_0^2},\quad
Q=\frac{\kappa a_0}{\pi G\Sigma}.
$$

Thus **$Q>1$ gives local axisymmetric oscillatory stability; $Q<1$ gives a growing band**, with

$$
q_-<q<q_+,\qquad
q_\pm=\frac{\pi G\Sigma}{a_0^2}\left(1\pm\sqrt{1-Q^2}\right).
$$

At $Q=1$, the minimizing mode has zero [frequency](../../../../frequency.md) and is marginal, not a strictly restoring oscillation. Local axisymmetric stability does not establish stability to every global nonaxisymmetric mode.

**[long-wave and short-wave branches at marginal Toomre stability](../../../../long-wave-and-short-wave-branches-at-marginal-toomre-stability.md).** For $Q=1$ and $n\geq1$,

$$
n^2(\Omega_P-\Omega)^2=(a_0q-\kappa)^2,
\qquad
q=\frac{\kappa\pm n|\Omega_P-\Omega|}{a_0}.
$$

The long-wavelength branch, using the minus sign, requires

$$
\boxed{\Omega-\frac\kappa n\leq\Omega_P\leq\Omega+\frac\kappa n}.
$$

These endpoints are the inner and outer [Lindblad resonance](../../../../lindblad-resonance.md) conditions. **The stated [dispersion relation](../../../../dispersion-relation-split.md) does not restrict every wave solution to that interval.** Its plus-sign short-wavelength branch has $q>0$ even outside it: for example, $\Omega_P=\Omega+2\kappa/n$ gives $q=3\kappa/a_0$ and satisfies the equation. Additional branch selection or resonant absorption physics would be needed for an absolute confinement claim. No such condition is supplied.

**[Toomre stability radius of a flat-rotation disk](../../../../toomre-stability-radius-of-a-flat-rotation-disk.md).** With $\Omega=v_0/r$, $\kappa=\sqrt2v_0/r$. Using $G=4.3009\times10^{-3}\ \mathrm{pc}\,(\mathrm{km\,s^{-1}})^2M_\odot^{-1}$,

$$
\boxed{Q(r)=\frac{\sqrt2v_0a_0}{\pi G\Sigma r}
\simeq\frac{4.19\ \mathrm{kpc}}r}.
$$

The supplied local model therefore predicts stable radii below about **$4.19\ \mathrm{kpc}$**, marginality at that radius, and axisymmetric instability farther out while its assumed constant [surface density](../../../../surface-density-of-a-disk.md) and thin-disk approximation remain applicable. An infinite constant-density, flat-rotation disk is an idealization, not a global self-consistent galaxy model.

<a id="2/image-original-marginal-disk-dispersion-branches-and-radial-toomre-parameter-showing-the-long-wave-restriction-and-the-surviving-short-wave-branch"></a>
![](../../../../past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2014/paper-1-disk-branches.png)

**[Figure 2](#2/image-original-marginal-disk-dispersion-branches-and-radial-toomre-parameter-showing-the-long-wave-restriction-and-the-surviving-short-wave-branch). Original marginal-disk dispersion branches and radial Toomre parameter, showing the long-wave restriction and the surviving short-wave branch**.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the formation of Structure in the Universe course of the University of Cambridge](../../../split.md)
5. [Formation of Structure in the Universe course of the University of Cambridge](../../../../formation-of-structure-in-the-universe-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
