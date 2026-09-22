<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Linearize about zero bulk flow and the uniform guide field. Put $\mathbf b=\delta\mathbf B/\sqrt{4\pi\rho}$, and take [plane waves](../../../../../../plane-wave.md) proportional to $e^{i(\mathbf k\cdot\mathbf x-\omega t)}$. Let $k_\parallel=\mathbf k\cdot\hat{\mathbf z}$, $k=|\mathbf k|$, $q=k_\parallel v_A$, and

$$
d_i=\frac c{\omega_{pi}},\qquad v_Ad_i=\frac{cB_0}{4\pi en}.
$$

Both $\mathbf u$ and $\mathbf b$ are perpendicular to $\mathbf k$. Projecting momentum onto that plane eliminates total [pressure](../../../../../../pressure.md). The remaining magnetic-tension term gives

$$
-i\omega\mathbf u=iq\mathbf b,\qquad \omega\mathbf u=-q\mathbf b.
$$

In the induction equation, the Hall contribution is $-c(B_0\partial_z)(\nabla\times\delta\mathbf B)/(4\pi en)$; its two derivative factors of $i$ in the [Fourier mode](../../../../../../fourier-mode.md) produce a positive coefficient multiplying $\mathbf k\times\mathbf b$. Thus

$$
-i\omega\mathbf b=iq\mathbf u+qd_i\mathbf k\times\mathbf b,
\qquad\omega\mathbf b=-q\mathbf u+i qd_i\mathbf k\times\mathbf b.
$$

Eliminating $\mathbf u$ gives

$$
(\omega^2-q^2)\mathbf b=i\omega qd_i\mathbf k\times\mathbf b.
$$

On the transverse plane, $(i\mathbf k\times)^2=k^2$, so applying that operator again proves the [incompressible Hall-MHD wave dispersion](../../../../../../incompressible-hall-mhd-wave-dispersion.md):

$$
\boxed{(\omega^2-k_\parallel^2v_A^2)^2=\omega^2 k_\parallel^2v_A^2k^2\frac{c^2}{\omega_{pi}^2}.}
$$

Equivalently, in a [helicity decomposition of a transverse Fourier mode](../../../../../../helicity-decomposition-of-a-transverse-fourier-mode.md) with $i\mathbf k\times\mathbf b_h=hk\mathbf b_h$, $h=\pm1$, each polarization obeys $\omega^2-hqkd_i\omega-q^2=0$. For $k_\parallel=0$ the projected linear restoring terms vanish and these modes have zero frequency; the propagating calculation assumes $k_\parallel\ne0$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
