<h1 id="s16/1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume ideal, nondegenerate particles in local thermodynamic equilibrium, ground-state atomic hydrogen, no molecules, and a common temperature. Let $\lambda_j=h/\sqrt{2\pi m_jk_BT}$ be the thermal [de Broglie wavelength](../../../../../de-broglie-wavelength.md). Choose zero energy for a separated stationary proton and electron, so a neutral atom has ground-state energy $-R$. The classical [chemical potentials](../../../../../chemical-potential-split.md) are

$$
\mu_e=k_BT\ln\frac{n_e\lambda_e^3}{g_e},\quad \mu_p=k_BT\ln\frac{n_p\lambda_p^3}{g_p},\quad \mu_H=-R+k_BT\ln\frac{n_H\lambda_H^3}{g_H}.
$$

Chemical equilibrium for $H\rightleftharpoons p+e$ requires $\mu_H=\mu_p+\mu_e$. Rearranging gives

$$
\frac{n_en_p}{n_H}=\frac{g_eg_p}{g_H}\frac{\lambda_H^3}{\lambda_e^3\lambda_p^3}e^{-R/(k_BT)}.
$$

Including electron and proton spin degeneracy, $g_e=2$, $g_p=2$ and $g_H=4$ when hyperfine splittings are neglected. Hence the statistical factor is one. Also $m_H\simeq m_p$, so $\lambda_H^3/\lambda_p^3\simeq1$. [Charge neutrality](../../../../../charge-neutrality.md) gives $n_p=n_e$, and therefore

$$
\boxed{\frac{n_e^2}{n_H}=\frac{(2\pi m_ek_BT)^{3/2}}{h^3}\exp\left(-\frac{R}{k_BT}\right).}
$$

This is the specified ground-state [Saha equation](../../../../../saha-ionization-equation.md). Keeping excited atomic partition functions or a different spin-counting convention can change a prefactor, so its convention must be stated rather than silently adding a factor of two. The left side has dimensions of a number density, not a dimensionless electron-to-neutral ratio.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [1](../../1.md)
3. [S16](../../../s16.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
