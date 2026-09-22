<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the first [lens](../../../../lens-optics.md), propagate, and apply the second [lens](../../../../lens-optics.md). Omitting only common prefactors and uniform [phases](../../../../phase-waves.md),

$$
E_{\mathrm{out}}(x)\propto\int dx'\,
\exp\!\left[-\frac{ikx^2}{2f}+\frac{ik(x-x')^2}{2L}-\frac{ikx'^2}{2f}\right]E_{\mathrm{in}}(x').
$$

The coefficients of both $x^2$ and $x'^2$ vanish if and only if $f=L$. The remaining cross term is $-ikxx'/L$, so

$$
\boxed{f=L,\qquad E_{\mathrm{out}}(x)\propto\int dx'\,e^{-i(kx/L)x'}E_{\mathrm{in}}(x')
=\widetilde E_{\mathrm{in}}\!\left(\frac{kx}{L}\right).}
$$

The Fourier convention here is $\widetilde E(q)=\int e^{-iqx}E(x)dx$. Finite clear apertures would truncate the field and limit the spatial-frequency range; the ideal relation assumes the paraxial field fits within both [lenses](../../../../lens-optics.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
