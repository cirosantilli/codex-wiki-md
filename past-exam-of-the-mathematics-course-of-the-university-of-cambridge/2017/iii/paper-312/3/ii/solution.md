<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a nonzero [Fourier mode](../../../../../../fourier-mode.md) $\mathbf k=k\hat z$, the divergence-free condition implies $B_z=0$. The complex vectors $m^{(\pm)}=(\hat x\pm i\hat y)/\sqrt2$ form a Hermitian orthonormal basis of this transverse plane. Their opposite rotation phases give the [helicity decomposition of a transverse Fourier mode](../../../../../../helicity-decomposition-of-a-transverse-fourier-mode.md); the factor $i/\sqrt2$ in the amplitudes is a convention. The baryon velocity in this vector sector has the analogous decomposition.

For [helicity](../../../../../../helicity.md) $\sigma=\pm1$, the angular source is

$$
\mathbf e\cdot\mathbf B^{(\sigma)}=\frac{i}{2}B^{(\sigma)}\sin\theta e^{i\sigma\varphi}=-\sigma i\sqrt{\frac{2\pi}{3}}B^{(\sigma)}Y_{1\sigma}.
$$

The same formula holds for $\mathbf v_b^{(\sigma)}$. Thus these sources have only angular order $m=\sigma$. Streaming multiplies by $ik\cos\theta$ and the stated [Thomson scattering](../../../../../../thomson-scattering.md) operator is diagonal in $m$, so neither mixes this sector with other angular orders. Assuming the initial anisotropy is in the same vector-helicity sector, or considering the anisotropy generated from zero initial data, the solution therefore contains only $Y_{\ell\sigma}$ with $\ell\geq1$. Arbitrary independently imposed anisotropies of other $m$ would instead evolve in their own homogeneous sectors.

There is a genuine normalization inconsistency in the PDF. To retain its printed temperature expansion, write

$$
\Theta^{(\sigma)}=\sum_{\ell\geq1}C_\ell q_\ell^{(\sigma)}Y_{\ell\sigma},\qquad C_\ell=(-i)^\ell\sqrt{\frac{2\ell+1}{8\pi}},
$$

where $q_\ell$ denotes exactly the multipoles called $\Theta_\ell$ in that expansion. The [spherical-harmonic streaming recurrence](../../../../../../spherical-harmonic-streaming-recurrence.md) gives the coefficient of $Y_{\ell\sigma}$ in $ik\cos\theta\,\Theta$, divided by $C_\ell$, as

$$
ik\left[\frac{C_{\ell+1}}{C_\ell}\sqrt{\frac{(\ell+1)^2-1}{(2\ell+3)(2\ell+1)}}q_{\ell+1}+\frac{C_{\ell-1}}{C_\ell}\sqrt{\frac{\ell^2-1}{(2\ell+1)(2\ell-1)}}q_{\ell-1}\right].
$$

Here $C_{\ell+1}/C_\ell=-i\sqrt{(2\ell+3)/(2\ell+1)}$ and $C_{\ell-1}/C_\ell=i\sqrt{(2\ell-1)/(2\ell+1)}$. Both streaming denominators are therefore $2\ell+1$, rather than the PDF's $2\ell+3$ and $2\ell-1$. The dipole source also changes: $C_1=-i\sqrt{3/(8\pi)}$, so $-(\mathbf e\cdot\dot{\mathbf B}+\dot\tau\mathbf e\cdot\mathbf v_b)/C_1$ is $-\sigma(4\pi/3)(\dot B^{(\sigma)}+\dot\tau v_b^{(\sigma)})Y_{1\sigma}$. The quadrupole collision correction is still $-\dot\tau q_2\delta_{\ell2}/10$.

Thus the [vector photon Boltzmann hierarchy](../../../../../../vector-photon-boltzmann-hierarchy.md) consistent with the literal printed expansion is

$$
\boxed{\dot q_\ell^{(\sigma)}+\frac{k}{2\ell+1}\left[\sqrt{(\ell+1)^2-1}\,q_{\ell+1}^{(\sigma)}-\sqrt{\ell^2-1}\,q_{\ell-1}^{(\sigma)}\right]=\dot\tau\left(1-\frac{\delta_{\ell2}}{10}\right)q_\ell^{(\sigma)}-\sigma\frac{4\pi}{3}(\dot B^{(\sigma)}+\dot\tau v_b^{(\sigma)})\delta_{\ell1}.}
$$

A concrete counterexample to the printed hierarchy with this expansion is a collisionless instant with $q_2=1$ and every other multipole zero. Direct streaming gives $\dot q_1=-k\sqrt3/3$, whereas the printed hierarchy would give $-k\sqrt3/5$.

Alternatively, preserve the PDF's desired hierarchy by making the [photon multipole normalization change](../../../../../../photon-multipole-normalization-change.md)

$$
\widetilde\Theta_\ell^{(\sigma)}=\frac{2\ell+1}{4\pi}q_\ell^{(\sigma)},\qquad \Theta^{(\sigma)}=\sum_{\ell\geq1}(-i)^\ell\sqrt{\frac{2\pi}{2\ell+1}}\,\widetilde\Theta_\ell^{(\sigma)}Y_{\ell\sigma}.
$$

This is the reciprocal angular normalization, not the printed expansion. Multiplying the corrected hierarchy by $(2\ell+1)/(4\pi)$ gives precisely

$$
\boxed{\dot{\widetilde\Theta}_\ell^{(\sigma)}+k\left[\frac{\sqrt{(\ell+1)^2-1}}{2\ell+3}\widetilde\Theta_{\ell+1}^{(\sigma)}-\frac{\sqrt{\ell^2-1}}{2\ell-1}\widetilde\Theta_{\ell-1}^{(\sigma)}\right]=\dot\tau\left(1-\frac{\delta_{\ell2}}{10}\right)\widetilde\Theta_\ell^{(\sigma)}-\sigma(\dot B^{(\sigma)}+\dot\tau v_b^{(\sigma)})\delta_{\ell1}.}
$$

This supplies both consistent conventions explicitly. The lower coupling vanishes at $\ell=1$, so no vector monopole is introduced. [Cosmological optical depth](../../../../../../cosmological-optical-depth.md) to the observer has $\dot\tau<0$, giving damping of the dipole and the factor $9/10$ quadrupole damping in this temperature-only collision model; no polarization collision term has been added to the supplied equation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
