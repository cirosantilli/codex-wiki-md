<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Free propagation is [convolution](../../../../convolution.md) with a chirp, $K_L(x)=C_Le^{ikL}e^{ikx^2/(2L)}$. The [convolution theorem](../../../../convolution-theorem.md) therefore turns it into multiplication by its [Fourier transform](../../../../fourier-transform-split.md). Complete the square:

$$
\frac{kx^2}{2L}-qx=\frac{k}{2L}\left(x-\frac{Lq}{k}\right)^2-\frac{Lq^2}{2k}.
$$

The [Gaussian integral](../../../../gaussian-integral.md) then gives

$$
\widetilde E(q,L)=C_L\sqrt{\frac{2\pi iL}{k}}\,
 e^{ikL-iLq^2/(2k)}\widetilde E(q,0).
$$

Thus the wavevector-dependent [phase](../../../../phase-waves.md) is

$$
\boxed{\varphi(k_\perp)=kL-\frac{Lk_\perp^2}{2k},}
$$

up to an overall [phase](../../../../phase-waves.md) convention; after removing the carrier it is $-Lk_\perp^2/(2k)$. This also follows from $k_z=\sqrt{k^2-k_\perp^2}\simeq k-k_\perp^2/(2k)$.

**[Normalization](../../../../normalization.md) qualification:** the source keeps a two-dimensional-style prefactor while integrating over only one transverse coordinate. With its literal $C_L=ik/(2\pi L)$, there is an additional $q$-independent factor, rather than solely a unit-modulus multiplier. A properly normalized one-dimensional [Fresnel propagator](../../../../fresnel-propagator.md) has $C_L=\sqrt{k/(2\pi iL)}$, which cancels the square-root factor above and makes propagation a pure Fourier-domain [phase](../../../../phase-waves.md). For example, the literal source kernel multiplies a plane-wave Fourier mode by a factor of magnitude $\sqrt{k/(2\pi L)}$, not one. The spatially dependent [phase](../../../../phase-waves.md) and the proportional Fourier-transform results remain unchanged. [Wave optics, two-dimensional Fourier optics: optical-path expansion and Fourier-domain diffraction](../../../../oscillations-and-waves-by-richard-fitzpatrick.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
