# Energy density and flux of a plane electromagnetic wave

↑ **Parent:** [Poynting theorem](poynting-theorem.md)

For a single traveling vacuum [plane electromagnetic wave](plane-electromagnetic-wave.md), $\mathbf B=\widehat{\mathbf k}\times\mathbf E/c$ gives equal electric and magnetic contributions to [electromagnetic energy](electromagnetic-energy.md):

$$
u_E=u_B=\frac12\epsilon_0|\mathbf E|^2,\qquad
u=\epsilon_0|\mathbf E|^2,\qquad
\mathbf S=cu\widehat{\mathbf k}.
$$

For the fields with [linear polarization](linear-polarization.md) along $x$ and magnetic orientation along $y$ specified above,

$$
\mathbf S(z,t)=\epsilon_0cE_0^2\cos^2(kz-\omega t)\widehat{\mathbf z},\qquad
\langle\mathbf S\rangle=\frac{\epsilon_0cE_0^2}{2}\widehat{\mathbf z}.
$$

Angle brackets mean an average over one period at fixed position. The factor $1/2$ comes from averaging squared [cosine](cosine.md); $E_0$ is the peak amplitude, whereas the [root mean square](root-mean-square.md) field is $E_{\mathrm{rms}}=E_0/\sqrt2$. The equal energy contributions oscillate together, rather than trading energy as in an [RLC circuit](rlc-circuit.md). [MIT 6.013 course notes, §2.7.3: power and energy in uniform plane waves](https://live.ocw.mit.edu/courses/6-013-electromagnetics-and-applications-spring-2009/d3be4ea78b036a6362230fb41780cf54_MIT6_013S09_notes.pdf).

For $E_0=100\,\mathrm{V/m}$, using $c=299792458\,\mathrm{m/s}$ and $\epsilon_0\simeq8.854\times10^{-12}\,\mathrm{F/m}$,

$$
B_0=\frac{100}{c}\,\mathrm{V/m}\simeq3.34\times10^{-7}\,\mathrm T,
\qquad
\langle S_z\rangle\simeq13.3\,\mathrm{W/m^2},
\qquad
\langle u\rangle\simeq4.43\times10^{-8}\,\mathrm{J/m^3}.
$$

A $0.010\,\mathrm{m^2}$ surface normal to $+z$ therefore has average crossing [power](power.md) $0.133\,\mathrm W$. This is incident [power](power.md); the amount absorbed depends on the surface. Doubling the field amplitude quadruples the average flux.

## ↑ Ancestors (7)

1. [Poynting theorem](poynting-theorem.md)
2. [Poynting vector](poynting-vector.md)
3. [Electromagnetic wave](electromagnetic-wave.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1/15d/d/solution.md)
