<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose longitudinal current along $x$, [magnetic field](../../../../magnetic-field-split.md) along $z$, and define the oriented [Hall coefficient](../../../../hall-coefficient.md) by $R_H=E_y/(j_xB_z)$. For one carrier type with signed charge $q$, a stationary transverse force balance is $q(\mathbf E+\mathbf v\times\mathbf B)_y=0$. Since $(\mathbf v\times\mathbf B)_y=-v_xB_z$, this gives $E_y=v_xB_z$. Using $j_x=nqv_x$,

$$
\boxed{R_H=\frac1{nq}},\qquad R_H=-\frac1{ne}\ \text{for electrons},\quad R_H=+\frac1{pe}\ \text{for holes}.
$$

This is the weak-field isotropic one-carrier approximation with [Hall scattering factor](../../../../hall-scattering-factor.md) one, not a general multiband identity.

Under the stipulated electron-dominated approximation, the given Hall magnitudes imply

$$
n_i(300)=\frac1{e(625)}=9.99\times10^{15}\ \mathrm{m^{-3}},\qquad
n_i(500)=4\times10^4n_i(300)=3.99\times10^{20}\ \mathrm{m^{-3}}.
$$

Take the ratio of the intrinsic activation law:

$$
4\times10^4=\left(\frac{500}{300}\right)^{3/2}
\exp\left[\frac{E_g}{2k_B}\left(\frac1{300}-\frac1{500}\right)\right].
$$

Solving gives the model's activation-gap estimate

$$
\boxed{E_g=\frac{2k_B\ln[4\times10^4(300/500)^{3/2}]}{1/300-1/500}
=2.04\times10^{-19}\ \mathrm J=1.27\ \mathrm{eV}}.
$$

This result uses the supplied Hall-temperature ratio and the fixed-gap, fixed-prefactor assumptions. A temperature-dependent gap or changing Hall factors would modify its interpretation.

The source's description of [electrons](../../../../electron.md) as intrinsic silicon's majority carriers needs qualification. **Intrinsic neutrality gives equal [electron](../../../../electron.md) and hole concentrations**, not an [electron density](../../../../electron-density.md) majority. [Electrons](../../../../electron.md) can nevertheless dominate conductivity and the Hall response because their mobility is larger. For two weak-field carriers,

$$
R_H=\frac{p\mu_h^2-n\mu_e^2}{e(p\mu_h+n\mu_e)^2}.
$$

At $n=p=n_i$ this becomes $R_H=-(\mu_e-\mu_h)/[en_i(\mu_e+\mu_h)]$. Thus $\mu_e>\mu_h$ explains the negative sign, while the one-electron formula is quantitatively accurate only if the hole contribution can be neglected. Equality $n=p$ itself is a concrete counterexample to a literal electron-number-majority claim. The numerical deductions above retain the approximation explicitly requested by the source.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
