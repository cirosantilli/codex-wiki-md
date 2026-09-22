<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take a long periodic section of length $L$, or neglect end effects and choose an integer number of wavelengths. The amplitude $u_q$ here is a single real sine amplitude, fixing the normalization of the [thermal membrane undulation](../../../../../thermal-membrane-undulation.md) spectrum. For a [lipid vesicle](../../../../../lipid-vesicle.md) with an [axisymmetric membrane deformation](../../../../../axisymmetric-membrane-deformation.md), conservation of the enclosed volume gives

$$
\pi\int_0^L R(z)^2\,dz=\pi L\left(\rho_0^2+\frac{u_q^2}{2}\right)=\pi LR_0^2,
\qquad
\rho_0=\sqrt{R_0^2-u_q^2/2}=R_0-\frac{u_q^2}{4R_0}+O(u_q^4).
$$

The mean radius therefore decreases at second order. This adjustment is essential: fixing the mean radius instead of the volume would miss the unstable term in the [fixed-volume capillary spectrum of a cylindrical membrane](../../../../../fixed-volume-capillary-spectrum-of-a-cylindrical-membrane.md).

The [surface area](../../../../../surface-area.md) of an axisymmetric graph is $\mathcal S=2\pi\int R\sqrt{1+R_z^2}\,dz$. Expanding for $|u_q|\ll R_0$ and $q|u_q|\ll1$ gives

$$
\mathcal S=2\pi L\rho_0+\frac{\pi LR_0}{2}q^2u_q^2+O(u_q^4)
=2\pi LR_0+\frac{\pi L}{2R_0}\bigl[(qR_0)^2-1\bigr]u_q^2+O(u_q^4).
$$

Multiplication by the [membrane tension](../../../../../membrane-tension.md) yields a quadratic [potential energy](../../../../../potential-energy.md) $\Delta E=K_q u_q^2/2$, where

$$
K_q=\frac{\pi\sigma L}{R_0}\bigl[(qR_0)^2-1\bigr].
$$

For $qR_0>1$, the [equipartition theorem](../../../../../equipartition-theorem.md) gives the stable-mode [fixed-volume capillary spectrum of a cylindrical membrane](../../../../../fixed-volume-capillary-spectrum-of-a-cylindrical-membrane.md)

$$
\boxed{\langle u_q^2\rangle=\frac{k_BT R_0}{\pi\sigma L\bigl[(qR_0)^2-1\bigr]}.}
$$

Here $k_B$ is the [Boltzmann constant](../../../../../boltzmann-constant.md) and $T$ is the [temperature](../../../../../temperature.md). The cosine amplitude has the same variance and is an independent real coordinate at quadratic order. If instead $R-\rho_0=\sum_{q\ne0}a_qe^{iqz}$ with $a_{-q}=a_q^*$, the corresponding positive-$q$ complex coefficient has $\langle|a_q|^2\rangle=k_BT R_0/[2\pi\sigma L((qR_0)^2-1)]$. This is the same [thermal membrane undulation](../../../../../thermal-membrane-undulation.md) spectrum in a different [Fourier mode](../../../../../fourier-mode.md) normalization.

For $qR_0<1$, **the cylinder is unstable rather than having a negative fluctuation variance**. The quadratic [surface area](../../../../../surface-area.md) change is negative: a sufficiently long-wavelength modulation reduces area while retaining volume. This is the [Rayleigh–Plateau instability](../../../../../rayleigh-plateau-instability.md), expressed here as pearling of a tension-dominated [lipid vesicle](../../../../../lipid-vesicle.md). A cylinder supporting such modes has no unconstrained harmonic [thermal equilibrium](../../../../../thermal-equilibrium.md) about the uniform state. The $q=0$ uniform radius change is forbidden by fixed volume, and $qR_0=1$ is marginal in the tension-only approximation. The finite length and endpoint constraints determine which nonzero [Fourier modes](../../../../../fourier-mode.md) are allowed.

The large [membrane tension](../../../../../membrane-tension.md) assumption controls modes with $qR_0$ of order one. For large $q$ the omitted [membrane bending modulus](../../../../../membrane-bending-modulus.md) contribution grows approximately as $\kappa q^4$ and overtakes the tension term when $\kappa q^2\gtrsim\sigma$. Thus the displayed tension-only spectrum requires $q\ll\sqrt{\sigma/\kappa}$ as well as small amplitudes and a positive stiffness. Close enough to the marginal wavelength, bending corrections must also be retained; their relative scale at $qR_0$ of order one is $\kappa/(\sigma R_0^2)$.

For the circular phase boundary in a [lipid bilayer](../../../../../lipid-bilayer.md), the energy is its perimeter times the [line tension](../../../../../line-tension.md) $\gamma$. Let $\varphi$ be the polar angle and write $r(\varphi)=\rho_0+u_m\sin(m\varphi)$, where the periodicity requires an integer $m=qR_0\ge1$. Fixed enclosed area implies

$$
\frac12\int_0^{2\pi}r^2\,d\varphi=\pi\left(\rho_0^2+\frac{u_m^2}{2}\right)=\pi R_0^2,
\qquad \rho_0=R_0-\frac{u_m^2}{4R_0}+O(u_m^4).
$$

The perimeter, including the mean-radius change, is

$$
\mathcal P=\int_0^{2\pi}\sqrt{r^2+r_\varphi^2}\,d\varphi
=2\pi R_0+\frac{\pi}{2R_0}(m^2-1)u_m^2+O(u_m^4).
$$

Thus the [fixed-area capillary spectrum of a circular boundary](../../../../../fixed-area-capillary-spectrum-of-a-circular-boundary.md), again for a single real sine or cosine amplitude, is

$$
\boxed{\langle u_m^2\rangle=\frac{k_BT R_0}{\pi\gamma(m^2-1)}
=\frac{k_BT R_0}{\pi\gamma((qR_0)^2-1)},\qquad m\ge2.}
$$

The complex [Fourier mode](../../../../../fourier-mode.md) coefficient convention again divides this result by two. The mode $m=0$ is excluded by the fixed-area constraint, so the negative-stiffness interval $0<m<1$ is not an allowed mode of a closed circular boundary.

At $qR_0=1$, the zero stiffness is the [translation mode of a circular boundary](../../../../../translation-mode-of-a-circular-boundary.md), not a shape instability. Displacing the centre by a small distance $h$ changes the radius to first order by $h\cos\varphi$ or $h\sin\varphi$ while leaving area and perimeter unchanged. For example, an exactly translated circle has

$$
r(\varphi)=h\cos\varphi+\sqrt{R_0^2-h^2\sin^2\varphi}
=R_0+h\cos\varphi-\frac{h^2}{4R_0}+\frac{h^2}{4R_0}\cos(2\varphi)+O(h^4).
$$

The higher harmonics complete a true [translation mode of a circular boundary](../../../../../translation-mode-of-a-circular-boundary.md). **The $m=1$ denominator therefore represents free centre motion:** an unconfined domain's centre has no restoring [force](../../../../../force.md) or finite equilibrium variance in an infinite membrane. Radius fluctuations about a recentered domain omit this mode; external confinement would give it a separate restoring stiffness.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
