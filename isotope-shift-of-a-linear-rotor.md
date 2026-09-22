# Isotope shift of a linear rotor

↑ **Parent:** [Linear rigid rotor](linear-rigid-rotor.md)

Changing an [isotope](isotope.md) changes a [mass](mass.md) and therefore the [moment of inertia](moment-of-inertia.md). If the [bond length](bond-length.md) is held fixed, $B\propto1/\mu$ and every corresponding transition shifts by the same fractional amount. This leading inverse-[reduced mass](reduced-mass.md) scaling is also used in the more complete diatomic formulation.[§2a, equations (4)–(5): isotope dependence of rotational constants and reduced mass](diatomic-spectral-database-by-national-institute-of-standards-and-technology/1-sigma-ground-state-molecules.md)

For a deliberately stipulated [carbon monoxide](carbon-monoxide.md) example, take $m_{12}=12u$, $m_{13}=13u$, $m_{16}=16u$, $u=1.66053906660\times10^{-27}\,\mathrm{kg}$, $r=1.13\times10^{-10}\,\mathrm m$ for both isotopic forms, and $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$. The integer [masses](mass.md) are simplifying inputs, not accurate isotopic atomic [masses](mass.md); the shared [bond length](bond-length.md) is an imposed model assumption. Calculation gives

$$
\begin{aligned}
\mu_{12,16}&=\frac{48}{7}u,& I_{12,16}&\approx1.45395\times10^{-46}\,\mathrm{kg\,m^2},& B_{12,16}&\approx57.7188\,\mathrm{GHz},\\
\mu_{13,16}&=\frac{208}{29}u,& I_{13,16}&\approx1.52080\times10^{-46}\,\mathrm{kg\,m^2},& B_{13,16}&\approx55.1817\,\mathrm{GHz}.
\end{aligned}
$$

In particular,

$$
\frac{B_{13,16}}{B_{12,16}}=\frac{\mu_{12,16}}{\mu_{13,16}}=\frac{87}{91}\approx0.956044.
$$

The heavier form's calculated $J=0\to1$ line is $110.363\,\mathrm{GHz}$ rather than $115.438\,\mathrm{GHz}$, a decrease of about $4.396\%$. These are model predictions from the stated inputs, not published measured [frequencies](frequency.md). An [isotope](isotope.md) changes the spacing as well as the first line; the shift is not a fixed additive offset for the whole spectrum.

<a id="image-molecular-rotation-isotope-and-distortion-spectra"></a>
![](molecular-rotation-isotope-and-distortion-spectra.png)

**[Figure 4](#image-molecular-rotation-isotope-and-distortion-spectra). Synthetic rotational spectroscopy comparison: a heavier isotope compresses the rigid spectrum, while centrifugal distortion bends the spacing pattern**. Original equal-height sticks for $J=0\to1$ through $4\to5$, using only the stipulated [masses](mass.md) and [bond length](bond-length.md) above. The lower panel additionally stipulates $D/B=0.001$ for the lighter form and compares $2B(J+1)-4D(J+1)^3$ with dashed rigid positions. Neither heights, distortion constant nor line [frequencies](frequency.md) are measured data; no thermal-population or instrument model is included.

## ↑ Ancestors (6)

1. [Linear rigid rotor](linear-rigid-rotor.md)
2. [Rigid rotor](rigid-rotor.md)
3. [Molecular rotation](molecular-rotation.md)
4. [Molecule](molecule-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Rotational spectral line assignment](rotational-spectral-line-assignment.md)
- [Rotational spectroscopy](rotational-spectroscopy.md)
