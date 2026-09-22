<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Neglect [electron mass](../../../../electron-mass.md) and nuclear binding corrections when converting [mass density](../../../../density.md) $\rho$ into [hydrogen](../../../../hydrogen.md) and [helium](../../../../helium.md) [number densities](../../../../number-density.md). With $x=x_H$,

$$
n_H=\frac{x\rho}{m_p},\qquad n_{\rm He}=\frac{(1-x)\rho}{4m_p},\qquad
n_e=n_H+2n_{\rm He}=\frac{(1+x)\rho}{2m_p}.
$$

The [thermal free-free emissivity](../../../../thermal-free-free-emissivity.md) adds over ion species with weights $Z_i^2$. Consequently

$$
\sum_i Z_i^2n_i=n_H+4n_{\rm He}=\frac\rho{m_p}=\frac{2n_e}{1+x}.
$$

With each [Gaunt factor](../../../../gaunt-factor.md) set to one, the mixture has

$$
\boxed{j_\nu=j_0\frac{2}{1+x_H}
\left(\frac{n_e}{10^{-3}\,\mathrm{cm}^{-3}}\right)^2
\sqrt{\frac{T_0}{T}}e^{-h\nu/(k_BT)}.}
$$

At fixed $n_e$, pure [hydrogen](../../../../hydrogen.md) gives the composition factor $1$, and pure [helium](../../../../helium.md) gives $2$. The latter check follows independently from $n_{\rm He}=n_e/2$ and $Z^2=4$; simply replacing $Z$ by an average charge would lose this weighting.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the radiative processes and high energy astrophysics course of the University of Oxford](../../../split.md)
5. [Radiative processes and high energy astrophysics course of the University of Oxford](../../../../radiative-processes-and-high-energy-astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
