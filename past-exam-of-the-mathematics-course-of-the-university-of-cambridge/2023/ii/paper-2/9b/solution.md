<h1 id="9b/solution">Solution</h1>

↑ **Parent:** [9B](../9b.md)

The given formula is the integral of the [Planck photon distribution](../../../../../planck-photon-distribution.md). Set

$$
x=\frac{h\nu}{k_BT},
\qquad d\nu=\frac{k_BT}{h}\,dx.
$$

Then

$$
n=\frac{8\pi}{c^3}\left(\frac{k_B}{h}\right)^3T^3
\int_0^\infty\frac{x^2}{e^x-1}\,dx
=\alpha T^3,
$$

where

$$
\alpha=\frac{8\pi}{c^3}\left(\frac{k_B}{h}\right)^3
\int_0^\infty\frac{x^2}{e^x-1}\,dx.
$$

Each photon of frequency $\nu$ has energy $h\nu$, so the energy density is

$$
\begin{aligned}
\rho
&=\frac{8\pi h}{c^3}\int_0^\infty
\frac{\nu^3}{e^{h\nu/(k_BT)}-1}\,d\nu\\
&=\frac{8\pi k_B^4}{c^3h^3}T^4
\int_0^\infty\frac{x^3}{e^x-1}\,dx
=\xi T^4.
\end{aligned}
$$

This is the [temperature scaling of thermal photon number and energy densities](../../../../../temperature-scaling-of-thermal-photon-number-and-energy-densities.md).

After decoupling, [cosmological redshift](../../../../../cosmological-redshift.md) gives

$$
\nu(t)=\frac{a(t_{\rm dec})}{a(t)}\nu_{\rm dec},
\qquad
\nu_{\rm dec}=\frac{a(t)}{a(t_{\rm dec})}\nu(t).
$$

The occupation number is conserved along the freely propagating photon trajectory. Its exponential argument at decoupling becomes

$$
\frac{h\nu_{\rm dec}}{k_BT_{\rm dec}}
=\frac{h\nu(t)}{k_B\bigl(a(t_{\rm dec})T_{\rm dec}/a(t)\bigr)}.
$$

Thus the spectrum still has the Planck form if

$$
\boxed{T(t)=\frac{a(t_{\rm dec})}{a(t)}T_{\rm dec}}.
$$

Frequency and temperature redshift by the same factor, which is the [redshift preservation of a thermal photon spectrum](../../../../../redshift-preservation-of-a-thermal-photon-spectrum.md).

## ↑ Ancestors (10)

1. [9B](../9b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
