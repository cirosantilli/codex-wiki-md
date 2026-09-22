<h1 id="section-b/8/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

There is a verified inconsistency in the printed data: the original PDF says $0.025\ \mathrm{nm}$, whereas the relativistic [de Broglie wavelength](../../../../../../de-broglie-wavelength.md) at $200\ \mathrm{kV}$ is approximately $0.00251\ \mathrm{nm}$:

$$
\lambda=\frac{h}{\sqrt{2m_e eV\left(1+eV/(2m_ec^2)\right)}}.
$$

Use consistent [length](../../../../../../length.md) units, $C_S=1.2\times10^6\ \mathrm{nm}$, and distinguish literal arithmetic from a physically consistent estimate. The familiar approximate [Scherzer defocus](../../../../../../scherzer-defocus.md) is $\Delta f_S\simeq-1.2\sqrt{C_S\lambda}$, or about **$-66\ \mathrm{nm}$** with $\lambda=0.0025\ \mathrm{nm}$. Slightly different optimum-phase conventions use $\sqrt{4/3}$ in place of $1.2$, giving about $-63\ \mathrm{nm}$; both are underfocus by a few tens of nanometres. The manufacturer's tabulated $200\ \mathrm{kV}$ values confirm that scale.[glossary, underfocus convention and accelerating-voltage/spherical-aberration table](../../../../../../scherzer-focus-by-jeol.md)

Using the question's additional numerical relation exactly as supplied, with $u=1/(0.22\ \mathrm{nm})$, gives

$$
\Delta f=\frac{0.54-\tfrac12 C_S\lambda^3u^4}{\lambda u^2}.
$$

For the physically appropriate rounded wavelength this is **$\Delta f\simeq-67.0\ \mathrm{nm}$**. The CTF itself gives an independent check: its first nonzero zero satisfies $\tfrac12 C_S\lambda^3u_0^4+\Delta f\lambda u_0^2=0$, so $u_0\simeq4.0\ \mathrm{nm^{-1}}$ implies **$\Delta f\simeq-60\ \mathrm{nm}$**. The plotted condition is therefore a little less underfocused than the usual Scherzer setting and has a first-zero spacing near $0.25\ \mathrm{nm}$. The nominal $0.22\ \mathrm{nm}$ and approximate optimization formula should not be treated as exactly reproducing every plotted parameter.

If the printed $0.025\ \mathrm{nm}$ is retained literally, the approximate Scherzer formula instead gives $-208\ \mathrm{nm}$, the supplied $0.54$ relation gives $-7.75\ \mathrm{\mu m}$, and the plotted first zero requires $-6.00\ \mathrm{\mu m}$. These do not describe a consistent $200\ \mathrm{kV}$ microscope. **The physically consistent comparison is approximately $-63$ to $-67\ \mathrm{nm}$ optimum underfocus versus $-60\ \mathrm{nm}$ from the plot; the wavelength correction is explicit.**

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [8](../../8.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
