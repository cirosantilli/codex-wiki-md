<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [polymer contour length](../../../../polymer-contour-length.md) and magnitude of total [electric charge](../../../../electric-charge-split.md) are

$$
L=20000(0.34\,\mathrm{nm})=6.80\,\mathrm{\mu m},\qquad
Q=\lambda L=40000e=6.409\times10^{-15}\,\mathrm C.
$$

Use a uniform charged-sphere model for the packed [DNA](../../../../deoxyribonucleic-acid.md), a homogeneous dielectric with $\epsilon=\epsilon_r\epsilon_0$, and initially neglect [electrostatic screening](../../../../electrostatic-screening.md). [Gauss's law](../../../../gauss-s-law.md) gives $E(r)=Qr/(4\pi\epsilon R^3)$ inside the sphere and $E(r)=Q/(4\pi\epsilon r^2)$ outside. Integrating the [electrostatic energy](../../../../electrostatic-energy.md) both inside and outside,

$$
U_c=\frac\epsilon2\int E^2\,dV
=\frac{Q^2}{40\pi\epsilon R}+\frac{Q^2}{8\pi\epsilon R}
=\boxed{\frac{3Q^2}{20\pi\epsilon R}}.
$$

For an illustrative aqueous relative [permittivity](../../../../permittivity-split.md) $\epsilon_r=80$ and $R=20\,\mathrm{nm}$,

$$
\boxed{U_c=1.384\times10^{-13}\,\mathrm J=1.384\times10^8\,\mathrm{pN\,nm}.}
$$

The question does not specify [permittivity](../../../../permittivity-split.md); the result scales as $80/\epsilon_r$. Using vacuum instead would increase it eightyfold and would not describe an aqueous interior.

Strictly, the [work](../../../../work.md) of packaging is a difference of [electrostatic energies](../../../../electrostatic-energy.md), rather than the packed self-energy alone. An extended charged rod also has self-energy. With a microscopic cutoff $a$ of order the [DNA](../../../../deoxyribonucleic-acid.md) radius, the thin-rod approximation is

$$
U_{\rm rod}\simeq\frac{\lambda^2L}{4\pi\epsilon}\left[\ln\left(\frac{2L}{a}\right)-1\right].
$$

One derivation integrates the pair [Coulomb potential](../../../../coulomb-potential-energy.md) along the rod, replacing separation by $\sqrt{z^2+a^2}$: the exact regularized expression is $\lambda^2[L\operatorname{arsinh}(L/a)-\sqrt{L^2+a^2}+a]/(4\pi\epsilon)$. The diagram's $1\,\mathrm{nm}$ transverse label suggests $a\simeq0.5\,\mathrm{nm}$, giving $U_{\rm rod}\simeq6.25\times10^6\,\mathrm{pN\,nm}$. Hence this explicit reference-state estimate is $\boxed{\Delta U\simeq1.32\times10^8\,\mathrm{pN\,nm}}$. The cutoff and precise initial conformation are additional model assumptions, but their correction is small compared with the unscreened sphere value.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
