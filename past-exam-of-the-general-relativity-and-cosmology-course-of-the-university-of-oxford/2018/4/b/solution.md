<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V$ be proper volume, let $g_i$ count the populated internal states, and take $\mu_i=0$ and $\epsilon=pc$. Spherical integration in momentum space gives

$$
\frac{N_i}{V}=\frac{g_i}{2\pi^2}\left(\frac{k_{\rm B}T}{\hbar c}\right)^3
\int_0^\infty\frac{x^2\,dx}{e^x\mp1},\qquad x=\frac{pc}{k_{\rm B}T}.
$$

Using the [fermion-to-boson thermal integral ratio](../../../../fermion-to-boson-thermal-integral-ratio.md), the minus-denominator [boson](../../../../boson.md) integral is $2\zeta(3)$ and the plus-denominator [fermion](../../../../fermion.md) integral is $3\zeta(3)/2$. Hence

$$
\boxed{N_B=\frac{g_B\zeta(3)}{\pi^2}V\left(\frac{k_{\rm B}T}{\hbar c}\right)^3,\qquad
N_F=\frac34\frac{g_F\zeta(3)}{\pi^2}V\left(\frac{k_{\rm B}T}{\hbar c}\right)^3.}
$$

The energy integral has one extra factor $pc=k_{\rm B}Tx$:

$$
\frac{U_i}{V}=\frac{g_i}{2\pi^2}\frac{(k_{\rm B}T)^4}{(\hbar c)^3}
\int_0^\infty\frac{x^3\,dx}{e^x\mp1}.
$$

The supplied distribution identity gives the [fermion](../../../../fermion.md) integral as $(1-2^{-3})\pi^4/15=7\pi^4/120$. Therefore

$$
\boxed{U_B=\frac{g_B\pi^2}{30}V\frac{(k_{\rm B}T)^4}{(\hbar c)^3},\qquad
U_F=\frac78\frac{g_F\pi^2}{30}V\frac{(k_{\rm B}T)^4}{(\hbar c)^3}.}
$$

For an isotropic [ultrarelativistic](../../../../ultrarelativistic-particle.md) gas, momentum flux gives $P_i=\tfrac13\int p v f_i\,d^3p$. Since $v=c$ and $pc=\epsilon$,

$$
\boxed{P_i=\frac{U_i}{3V}.}
$$

[Photons](../../../../photon.md) have $g_\gamma=2$, [electrons](../../../../electron.md) and [Positrons](../../../../positron.md) each have $g=2$, and each [neutrino](../../../../neutrino.md) or antineutrino species has one populated [helicity](../../../../helicity.md) in the standard thermal bath.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
