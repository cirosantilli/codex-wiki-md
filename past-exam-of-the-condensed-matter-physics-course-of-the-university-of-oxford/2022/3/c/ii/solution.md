<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The plateau in both source plots is approximately $10^{18.5}\,\mathrm{m^{-3}}$, so

$$
\boxed{N_D\simeq3\times10^{18}\,\mathrm{m^{-3}}.}
$$

These are graphical estimates, not high-precision fitted material parameters. To extract activation [energies](../../../../../energy-split.md) consistently with part (a), retain the [temperature](../../../../../temperature-split.md) powers in the [effective density of states](../../../../../effective-density-of-states.md) factors.

On the [semiconductor carrier freeze-out](../../../../../semiconductor-carrier-freeze-out.md) tail, put $x=1/T$. Then

$$
\log_{10}n=\text{constant}-\frac34\log_{10}x
-\frac{E_i}{2k_B\ln10}x.
$$

For example, the right-hand graph gives roughly $\log_{10}[n/(\mathrm{m^{-3}})]\simeq17.7$ at $x=0.10\,\mathrm{K^{-1}}$ and $13.0$ at $x=0.30\,\mathrm{K^{-1}}$. Subtract the known prefactor contribution before interpreting the slope:

$$
E_i\simeq2k_B\ln10\,
\frac{4.7-(3/4)\log_{10}3}{0.20\,\mathrm{K^{-1}}}
\simeq8.6\times10^{-3}\,\mathrm{eV}.
$$

Thus $\boxed{E_i\simeq9\,\mathrm{meV}}$, to the accuracy of the drawing. Ignoring the weak prefactor gives about $9.3\,\mathrm{meV}$, a similar rough estimate.

For the intrinsic branch, use

$$
\ln\frac{n(T_2)}{n(T_1)}=\frac32\ln\frac{T_2}{T_1}
+\frac{E_g}{2k_B}\left(\frac1{T_1}-\frac1{T_2}\right).
$$

The left-hand graph gives $n(100\,\mathrm K)\simeq2.5\times10^{21}\,\mathrm{m^{-3}}$ and $n(500\,\mathrm K)\simeq1.5\times10^{24}\,\mathrm{m^{-3}}$, both far above $N_D$. Therefore

$$
E_g\simeq\frac{2k_B\left[\ln600-(3/2)\ln5\right]}
{(1/100-1/500)\,\mathrm{K^{-1}}}
\simeq0.086\,\mathrm{eV},\qquad
\boxed{E_g\simeq0.09\,\mathrm{eV}.}
$$

Here $k_B=8.6173\times10^{-5}\,\mathrm{eV\,K^{-1}}$. Omitting the $T^{3/2}$ prefactor over this wide [temperature](../../../../../temperature-split.md) interval would instead give approximately $0.14\,\mathrm{eV}$, so it is not a negligible correction for the [band-gap extraction from intrinsic carrier activation](../../../../../band-gap-extraction-from-intrinsic-carrier-activation.md). The source graph warrants an approximate narrow [band gap](../../../../../band-gap.md), rather than several significant figures.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the condensed matter physics course of the University of Oxford](../../../../split.md)
6. [Condensed matter physics course of the University of Oxford](../../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
7. [Year 3 of the physics course of the University of Oxford](../../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
