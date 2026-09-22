<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use two [plane waves](../../../plane-wave.md), $|\mathbf k\rangle$ and $|\mathbf k-\mathbf G\rangle$, as a [basis](../../../basis.md) near their Bragg degeneracy. The potential has [Fourier coefficients](../../../fourier-coefficient.md) $V_{\pm\mathbf G}$; its zero [Fourier coefficient](../../../fourier-coefficient.md) vanishes. All other [plane waves](../../../plane-wave.md) are off [resonance](../../../resonance.md) and are neglected in the leading [nearly-free electron model](../../../nearly-free-electron-model.md). With $\varepsilon_{\mathbf k}=\hbar^2k^2/(2m_e)$, the [Schrödinger equation](../../../schrodinger-equation.md) reduces to the [Hermitian matrix](../../../hermitian-operator.md) problem

$$
\begin{pmatrix}
\varepsilon_{\mathbf k}&V_G\\
V_G^*&\varepsilon_{\mathbf k-\mathbf G}
\end{pmatrix}
\begin{pmatrix}c_1\\c_2\end{pmatrix}
=E\begin{pmatrix}c_1\\c_2\end{pmatrix}.
$$

Setting the [characteristic polynomial](../../../characteristic-polynomial.md) equal to zero gives

$$
(E-\varepsilon_{\mathbf k})(E-\varepsilon_{\mathbf k-\mathbf G})-|V_G|^2=0.
$$

Solving this [quadratic equation](../../../quadratic-equation.md) gives

$$
E_\pm=\frac{\varepsilon_{\mathbf k}+\varepsilon_{\mathbf k-\mathbf G}}2
\pm\sqrt{\left(\frac{\varepsilon_{\mathbf k}-\varepsilon_{\mathbf k-\mathbf G}}2\right)^2+|V_G|^2}.
$$

For the real [cosine](../../../cosine.md) potential its coefficient $V_G$ is real; the absolute-value form also allows an arbitrary choice of origin and corresponding Fourier phase.

At the Brillouin-zone boundary, $\mathbf k\cdot\mathbf G=G^2/2$, the free energies are equal. The two [standing waves](../../../standing-wave.md) have different [probability densities](../../../probability-density.md) relative to the [lattice](../../../lattice.md) potential and are split by

$$
\boxed{\Delta E=2|V_G|.}
$$

Repeating this [avoided crossing](../../../avoided-crossing.md) at the [reciprocal lattice](../../../reciprocal-lattice.md) boundaries joins smooth branches into [energy bands](../../../energy-band.md). In one dimension a nonzero [Fourier coefficient](../../../fourier-coefficient.md) opens a gap at the corresponding crossing. In higher dimensions a direct gap at one [wavevector](../../../wavevector.md) need not give a common forbidden [energy](../../../energy-split.md) interval at every [wavevector](../../../wavevector.md): different bands may still overlap in [energy](../../../energy-split.md). The present two-dimensional example remains metallic even though the crossings are locally gapped.

For the rectangular [lattice](../../../lattice.md), choose real-space primitive vectors $a\widehat{\mathbf x}$ and $b\widehat{\mathbf y}$. The [reciprocal lattice](../../../reciprocal-lattice.md) vectors are

$$
\mathbf G_x=\frac{2\pi}{a}\widehat{\mathbf x},\qquad
\mathbf G_y=\frac{2\pi}{b}\widehat{\mathbf y}.
$$

Define the half-widths of the first [Brillouin zone](../../../brillouin-zone.md) by $K=\pi/a$ and $L=\pi/b$. Their values and the zone are

$$
\boxed{K=2.41661\,\mathrm{nm^{-1}},\quad L=3.92699\,\mathrm{nm^{-1}},\quad
-K\leq k_x\leq K,\quad -L\leq k_y\leq L.}
$$

A primitive reciprocal cell can be drawn with a corner at the origin; its centred translate is the first [Brillouin zone](../../../brillouin-zone.md) here. Its area is $4\pi^2/(ab)=37.9600\,\mathrm{nm^{-2}}$.

<a id="3/image-real-space-primitive-cell-and-reciprocal-space-first-brillouin-zone"></a>
![](../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012-rectangular-cells.png)

**[Figure 4](#3/image-real-space-primitive-cell-and-reciprocal-space-first-brillouin-zone). Real-space primitive cell and reciprocal-space first Brillouin zone**.

Including both [spin](../../../spin.md) states, counting the occupied free-electron states per unit area gives

$$
n_{2D}=2\frac{\pi k_F^2}{(2\pi)^2}=\frac{k_F^2}{2\pi}
=\frac2{ab}.
$$

Consequently

$$
\boxed{k_F=\sqrt{\frac{4\pi}{ab}}=3.47607\,\mathrm{nm^{-1}},\qquad
E_F^{(0)}=\frac{\hbar^2k_F^2}{2m_e}=0.46036\,\mathrm{eV}.}
$$

The occupied [disk](../../../disk-mathematics.md) has precisely the area of the first [Brillouin zone](../../../brillouin-zone.md), but their shapes differ: $K<k_F<L$. It protrudes through both vertical zone boundaries and does not reach the horizontal ones. Thus two [electrons](../../../electron.md) per cell do not imply a filled first band in the absence of a separating [band gap](../../../band-gap.md).

Fold the protruding caps by $\pm\mathbf G_x$. The original [circle](../../../circle.md) and the translated [circle](../../../circle.md) intersect at $k_x=K$, $k_y=\pm\sqrt{k_F^2-K^2}$. The potential mixes these states and replaces each crossing by an [avoided crossing](../../../avoided-crossing.md). The lower branch reconnects into two open sheets running across successive zones in the $k_x$ direction; the upper branch forms a closed lens-shaped pocket about a vertical zone boundary. In a reduced-zone sketch its two halves sit at opposite edges, but periodic identification makes them **one closed sheet**. This is [rectangular-lattice Fermi-surface reconstruction](../../../rectangular-lattice-fermi-surface-reconstruction.md).

<a id="3/image-free-and-reconstructed-fermi-contours-two-open-sheets-and-one-closed-pocket-per-reciprocal-cell"></a>
![](../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2012-fermi-reconstruction.png)

**[Figure 5](#3/image-free-and-reconstructed-fermi-contours-two-open-sheets-and-one-closed-pocket-per-reciprocal-cell). Free and reconstructed Fermi contours: two open sheets and one closed pocket per reciprocal cell**.

The largest pocket in this weak-potential construction is the [lens-shaped intersection of two disks](../../../lens-shaped-intersection-of-two-disks.md) enclosed by the intersecting free circles. Each has radius $k_F$ and their centres are separated by $2K$. If $\theta=\arccos(K/k_F)$, two sectors minus their two triangles give the [lens bound on a reconstructed Fermi pocket](../../../lens-bound-on-a-reconstructed-fermi-pocket.md):

$$
A_{\max}=2k_F^2\theta-2K\sqrt{k_F^2-K^2},\qquad
\boxed{A_{\max}=7.30680\,\mathrm{nm^{-2}}.}
$$

Opening a gap raises the upper branch at fixed [chemical potential](../../../chemical-potential-split.md) and shrinks its pocket. The reported [quantum oscillation](../../../quantum-oscillation.md) area satisfies

$$
\boxed{0<A_k=5.74\,\mathrm{nm^{-2}}<A_{\max},\qquad
\frac{A_k}{A_{\max}}=0.786.}
$$

It is therefore consistent with this closed sheet. [Onsager quantization](../../../onsager-quantization.md) gives $F=\hbar A_k/(2\pi e)\simeq601\,\mathrm T$. An orbit on this closed contour can return to itself under the [Lorentz force](../../../lorentz-force.md) and occupy quantized [Landau levels](../../../landau-level.md). The open sheets do not enclose a finite orbit area for a perpendicular field in this two-dimensional model. The observation is consistent with the reconstructed pocket, without uniquely determining a completely arbitrary band structure.

For a quantitative rough coupling estimate, use the supplied fixed-chemical-potential approximation and retain the two waves coupled by $\mathbf G_x$. Write

$$
C=\frac{\hbar^2}{2m_e}=0.0380998\,\mathrm{eV\,nm^2},\qquad
v=|V_G|,\qquad k_x=K+q.
$$

Their upper [eigenvalue](../../../eigenvalue.md) is

$$
E_+(q,k_y)=C(K^2+q^2+k_y^2)+\sqrt{4C^2K^2q^2+v^2}.
$$

Setting it equal to $Ck_F^2$ gives the pocket boundary

$$
k_y^2=k_F^2-K^2-q^2-\sqrt{4K^2q^2+(v/C)^2}.
$$

Its intersection with $k_y=0$ occurs at $q=\pm q_m$, where

$$
q_m^2=k_F^2+K^2-\sqrt{4k_F^2K^2+(v/C)^2}.
$$

The [two-wave estimate of a Bragg-gap coupling from a pocket area](../../../two-wave-estimate-of-a-bragg-gap-coupling-from-a-pocket-area.md) therefore uses

$$
A(v)=4\int_0^{q_m}
\sqrt{k_F^2-K^2-q^2-\sqrt{4K^2q^2+(v/C)^2}}\,dq.
$$

At $v=0$ this reproduces the [lens bound on a reconstructed Fermi pocket](../../../lens-bound-on-a-reconstructed-fermi-pocket.md); the pocket disappears at $v=C(k_F^2-K^2)=0.23786\,\mathrm{eV}$. [Numerical integration](../../../numerical-integration-split.md) gives $A(0.075\,\mathrm{eV})=6.22\,\mathrm{nm^{-2}}$ and $A(0.100\,\mathrm{eV})=5.54\,\mathrm{nm^{-2}}$. Matching the measured area gives $v\simeq0.0931\,\mathrm{eV}$, so the justified rough result is

$$
\boxed{|V_G|\sim0.1\,\mathrm{eV}\qquad(\Delta E\sim0.2\,\mathrm{eV}).}
$$

This estimate neglects remote plane-wave admixtures and other [Fourier coefficients](../../../fourier-coefficient.md). It also holds the [chemical potential](../../../chemical-potential-split.md) fixed as requested; an exact fixed-density calculation would determine it self-consistently after reconstruction. The numerical root is a way to implement the approximate model, not a measurement of $V_G$ to four significant figures.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2012](../../2012-split.md)
3. [Past exam of the quantum condensed matter course of the University of Cambridge](../../split.md)
4. [Quantum Condensed Matter course of the University of Cambridge](../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
