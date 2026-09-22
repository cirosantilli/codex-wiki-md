# Circular-orbit derivation of the Bohr model

↑ **Parent:** [Bohr model](bohr-model.md)

Consider a single [electron](electron.md) of [mass](mass.md) $m_e$ and a point [atomic nucleus](atomic-nucleus-split.md) of [mass](mass.md) $M$ and positive [electric charge](electric-charge-split.md) $Ze$, with $e>0$ the [elementary charge](elementary-charge.md). Use nonrelativistic [classical mechanics](classical-mechanics-split.md), omit external fields and interactions with other [electrons](electron.md), and write

$$
\mu=\frac{m_eM}{m_e+M},\qquad
\kappa=\frac{Ze^2}{4\pi\epsilon_0},\qquad
\hbar=\frac{h}{2\pi}.
$$

Here $\mu$ is the [Coulomb two-body reduced mass](coulomb-two-body-reduced-mass.md), $\epsilon_0$ the [vacuum permittivity](vacuum-permittivity.md), and $h$ the [Planck constant](planck-constant.md). The separation $r$ and relative speed $v$ describe the [two-particle relative coordinate](two-particle-relative-coordinate.md); neither body is silently pinned in place. The [electron](electron.md)'s own radius about the [centre of mass](center-of-mass.md) is $Mr/(M+m_e)$.

For the assumed circular [orbit](orbit-dynamical-system.md), [Coulomb's law](coulomb-s-law.md) provides the required [centripetal acceleration](centripetal-acceleration.md), and the imposed [orbital angular momentum](orbital-angular-momentum.md) condition is

$$
\frac{\mu v^2}{r}=\frac{\kappa}{r^2},\qquad
L=\mu vr=n\hbar,\qquad n=1,2,3,\ldots.
$$

Substitute $v=n\hbar/(\mu r)$ into the first equation and cancel $r^{-2}$ to obtain

$$
r_n=\frac{n^2\hbar^2}{\mu\kappa},\qquad
v_n=\frac{\kappa}{n\hbar}.
$$

The [kinetic energy](kinetic-energy.md) is $K=\mu v^2/2=\kappa/(2r)$ and the [Coulomb potential energy](coulomb-potential-energy.md) is $U=-\kappa/r$, with zero [energy](energy-split.md) at infinite separation. Hence

$$
E_n=K+U=-\frac{\kappa}{2r_n}
=-\frac{\mu Z^2e^4}{2(4\pi\epsilon_0)^2\hbar^2n^2}.
$$

This derives the [energy](energy-split.md) sequence from the stated circular model; the modern [Schrödinger equation](schrodinger-equation.md) derivation is the distinct [series-termination quantization of the Coulomb radial equation](series-termination-quantization-of-the-coulomb-radial-equation.md). The radius above scales as $n^2/Z$, whereas the [binding energy](binding-energy.md) scales as $\mu Z^2/n^2$. The [Bohr radius](bohr-radius.md) article supplies the corresponding [Coulomb potential](coulomb-potential-energy.md) length scale. The nonrelativistic assumption requires $v_n\ll c$, with $c$ the [speed of light](speed-of-light.md).

For an original numerical example choose $Z=1$, $M=1.67262192369\times10^{-27}\,\mathrm{kg}$, $m_e=9.1093837015\times10^{-31}\,\mathrm{kg}$, $e=1.602176634\times10^{-19}\,\mathrm C$, $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$, $\epsilon_0=8.8541878128\times10^{-12}\,\mathrm{F\,m^{-1}}$, and $c=299792458\,\mathrm{m\,s^{-1}}$. Treat these as stipulated constants for the calculation. They give $\mu/m_e=0.99945568$, $r_1=0.0529465\,\mathrm{nm}$, $E_1=-13.598287\,\mathrm{eV}$ and $v_1/c\simeq0.00730$, where $\mathrm{eV}$ denotes an [electronvolt](electronvolt.md). At $n=2$, $r_2=4r_1$ and $E_2=E_1/4$; the ground-state [ionization energy](ionization-energy.md) is $-E_1$.

Taking $M\to\infty$ gives $\mu\to m_e$. A finite nuclear [mass](mass.md) reduces every [binding energy](binding-energy.md) by $\mu/m_e$ and increases each separation by $m_e/\mu$. This follows from relative motion, not a fitted correction to individual [spectral lines](spectral-line.md). Replacing the [atomic nucleus](atomic-nucleus-split.md) by a heavier [isotope](isotope.md) changes the same factor, providing another check of the model.

## ↑ Ancestors (5)

1. [Bohr model](bohr-model.md)
2. [Hydrogen atom](hydrogen-atom.md)
3. [Mathematical physics](mathematical-physics-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
