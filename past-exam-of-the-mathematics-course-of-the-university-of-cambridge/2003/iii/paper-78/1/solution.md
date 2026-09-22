<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

At normal incidence the [P wave](../../../../../p-wave.md) and the two [S wave](../../../../../s-wave.md) polarizations decouple. In each uniform layer the relevant displacement satisfies $\rho u_{tt}=C u_{zz}$, with $C=\lambda+2\mu$ for a longitudinal wave and $C=\mu$ for a shear wave. Its speed is $v=\sqrt{C/\rho}$ and its [seismic impedance](../../../../../seismic-impedance.md) is $Z=\rho v$. A welded interface preserves particle velocity and [traction](../../../../../traction.md). For displacement or velocity amplitudes, incidence from medium 0 onto medium 1 therefore gives

$$
1+r=t,\qquad Z_0(1-r)=Z_1t,
\qquad\boxed{r=\frac{Z_0-Z_1}{Z_0+Z_1},\quad t=\frac{2Z_0}{Z_0+Z_1}}.
$$

Reflection reverses the displacement sign when the receiving [seismic impedance](../../../../../seismic-impedance.md) is larger. The energy-flux fractions are

$$
\boxed{\mathcal R=|r|^2,\qquad\mathcal T=\frac{Z_1}{Z_0}|t|^2,\qquad\mathcal R+\mathcal T=1}.
$$

The impedance factor matters: a displacement [transmission coefficient](../../../../../transmission-coefficient.md) larger than one does not imply energy amplification. Equal impedance eliminates reflection even when the densities and speeds differ.

For a stack, every interface creates reflected waves which can return to all earlier interfaces. A [seismic layer transfer matrix](../../../../../seismic-layer-transfer-matrix.md) incorporates those multiple reflections exactly. Use harmonic time dependence $e^{-i\omega t}$, particle velocity $V$ and compressive [traction](../../../../../traction.md) $P=-\sigma_{zz}$ for a P-wave, or the negative relevant shear [traction](../../../../../traction.md) for an S-wave. Through layer $j$ of thickness $h_j$,

$$
\binom{V}{P}_{\!j,\mathrm{bottom}}=
M_j\binom{V}{P}_{\!j,\mathrm{top}},\qquad
M_j=\begin{pmatrix}\cos\delta_j&i\sin\delta_j/Z_j\\ iZ_j\sin\delta_j&\cos\delta_j\end{pmatrix},
\qquad\delta_j=\frac{\omega h_j}{v_j}.
$$

This follows by solving $V_z=i\omega P/C_j$ and $P_z=i\omega\rho_jV$. Continuity means that the state passes unchanged across each welded interface. Put $M=M_N\cdots M_1=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, with $ad-bc=1$, and let the exterior impedances be $Z_L,Z_R$. A unit incident velocity gives top state $(1+r,Z_L(1-r))$ and bottom state $(t,Z_Rt)$. Eliminating these states yields

$$
D=Z_Ra+Z_Ld-c-Z_LZ_Rb,
\qquad\boxed{r=\frac{c+Z_Ld-Z_Ra-Z_LZ_Rb}{D},\qquad t=\frac{2Z_L}{D}}.
$$

For real moduli and no attenuation, conservation of [elastic-wave energy flux](../../../../../elastic-wave-energy-flux.md) gives $|r|^2+(Z_R/Z_L)|t|^2=1$. Reciprocal incidence gives equal energy transmission in the reverse direction; flux-normalized amplitudes express that reciprocity without unequal exterior impedances obscuring it.

The [wave phase](../../../../../phase-waves.md) accumulated in each layer determines constructive or destructive interference. For one layer between identical exterior media, an integral number of half-wavelengths makes $M_j=\pm I$ and gives perfect transmission, regardless of the layer impedance. At quarter-wave phase thickness, a single matching layer with $Z_j=\sqrt{Z_LZ_R}$ also gives zero reflection: the layer transforms the terminal impedance to $Z_j^2/Z_R=Z_L$. Away from these matching conditions there are transmission peaks, reflection maxima and rapid [frequency](../../../../../frequency.md)-dependent phase changes. In the time domain these are a direct transmitted pulse followed by delayed internal reverberations and reflected echoes. Long residence in a resonant stack produces narrow peaks and long ringing, without creating energy.

For a periodic two-layer stack, the half-trace of one cell is

$$
\cos(Kd)=\cos\delta_1\cos\delta_2
-\frac12\left(\frac{Z_1}{Z_2}+\frac{Z_2}{Z_1}\right)\sin\delta_1\sin\delta_2.
$$

This is the [periodic seismic multilayer stop band](../../../../../periodic-seismic-multilayer-stop-band.md) criterion. When the absolute right side exceeds one, the cell [eigenvalues](../../../../../eigenvalue.md) are a reciprocal growing/decaying pair and a long finite stack has exponentially small transmission. The missing transmitted energy is reflected, not absorbed. Large impedance contrast and repeated quarter-wave layers strengthen such stop bands. In pass bands the cell modes propagate, and a finite stack superposes transmission resonances on that propagation. An irregular stack need not have equally spaced peaks: the individual travel times and impedance contrasts set its interference pattern.

At sufficiently low [frequency](../../../../../frequency.md) a finite stack has $M\to I$, so its leading reflection is that of the two exterior media alone. For many thin repeated layers with wavelength much longer than a cell, their effective density is the volume-weighted density and their normal modulus is the harmonic mean, $C_{\rm eff}^{-1}=\langle C^{-1}\rangle$. This follows by expanding each propagation matrix to first order and averaging its two coefficients. At high [frequency](../../../../../frequency.md), sharp interfaces still reflect: there is no general disappearance of reflection, only increasingly rapid interference fringes. Smooth impedance grading instead suppresses short-wavelength reflection when its variation scale is long compared with the wavelength.

These calculations provide a reproducible investigation: vary the layer travel times, impedances and number of cells; compute the matrix product; plot reflected/transmitted fluxes and check their sum. Adding attenuation makes the flux sum smaller than one and reduces reverberation peaks, while oblique incidence introduces [Snell law for elastic waves](../../../../../snell-law-for-elastic-waves.md) and P-SV mode conversion absent from this one-dimensional setting. **Impedance contrasts generate reflections, propagation phases organize their interference, and energy conservation separates reflection from genuine absorption**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
