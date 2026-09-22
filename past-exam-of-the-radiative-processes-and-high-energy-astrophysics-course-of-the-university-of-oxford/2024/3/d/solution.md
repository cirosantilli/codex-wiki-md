<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The coefficient $j_\nu$ is [power](../../../../power.md) per unit [volume](../../../../volume.md), [frequency](../../../../frequency.md) and [solid angle](../../../../solid-angle.md). For uniform, [optically thin](../../../../optically-thin-medium.md), [isotropic](../../../../isotropy.md) emission from $V=4\pi R^3/3$, the [spectral luminosity](../../../../spectral-luminosity.md) is $L_\nu=4\pi Vj_\nu$. With [photon](../../../../photon.md) [energy](../../../../energy-split.md) $\varepsilon=h\nu$, [conservation of energy](../../../../conservation-of-energy.md) and the change of spectral variable give

$$
L_\nu\,d\nu=\varepsilon L_\varepsilon^X\,d\varepsilon,
\qquad d\nu=\frac{d\varepsilon}{h}.
$$

Thus

$$
\boxed{L_\varepsilon^X=\frac{4\pi}{h\varepsilon}\frac{4\pi R^3}{3}
 j_0\frac{2}{1+x_H}
\left(\frac{n_e}{10^{-3}\,\mathrm{cm}^{-3}}\right)^2
\sqrt{\frac{T_0}{T}}e^{-\varepsilon/(k_BT)}.}
$$

The $4\pi$ outside $V$ integrates over emitted [solid angle](../../../../solid-angle.md); $1/\varepsilon$ changes radiated [energy](../../../../energy-split.md) to a [photon](../../../../photon.md) count, and $1/h$ is the [Jacobian determinant](../../../../jacobian-determinant.md) from [frequency](../../../../frequency.md) to [energy](../../../../energy-split.md).

With $h$ in $\mathrm{J\,s}$ and $\varepsilon$ in joules, this formula produces $\mathrm{J^{-1}\,s^{-1}}$. To compare with counts per $\mathrm{keV}$, multiply by $1.602176634\times10^{-16}\,\mathrm{J/keV}$. Equivalently, the conversion cancels the same joule-per-$\mathrm{keV}$ factor in $\varepsilon$: one can use the numerical $\varepsilon$ in $\mathrm{keV}$ in the $1/\varepsilon$ factor, retain $h$ in $\mathrm{J\,s}$, and express $k_BT$ in $\mathrm{keV}$ in the exponential. The radius in the [volume](../../../../volume.md) must still be converted to metres because $j_0$ is per $\mathrm{m^3}$.

## ↑ Ancestors (12)

1. [D](../d.md)
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
