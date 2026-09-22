<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the shown sequence of free space, [thin lens](../../../../thin-lens.md), and free space, multiply the [ray transfer matrices](../../../../ray-transfer-matrix-analysis.md) in traversal order:

$$
M=P(L_2)F(f)P(L_1)=\begin{pmatrix}
1-L_2/f&L_1+L_2-L_1L_2/f\\-1/f&1-L_1/f
\end{pmatrix}.
$$

To obtain an ordinary [Fourier transform](../../../../fourier-transform-split.md) of an arbitrary input field, neither an input quadratic [phase](../../../../phase-waves.md) nor an output quadratic [phase](../../../../phase-waves.md) may remain. Thus $A=D=0$, requiring

$$
\boxed{L_1=L_2=f,\qquad M=\begin{pmatrix}0&f\\-1/f&0\end{pmatrix}.}
$$

Using the physically consistent kernel derived in part b gives

$$
\boxed{E(x')=\frac{e^{ikL_0}}{\sqrt{i\lambda f}}\int E(x)e^{-i2\pi xx'/(\lambda f)}\,dx
=\frac{e^{ikL_0}}{\sqrt{i\lambda f}}\widehat E\!\left(\frac{x'}{\lambda f}\right).}
$$

The spatial Fourier coordinate is $x'/(\lambda f)$. If the source's schematic integral normalization is retained instead, set its slowly varying denominator to $L_0$ to obtain the same [Fourier transform](../../../../fourier-transform-split.md) with overall prefactor $ik e^{ikL_0}/(2\pi L_0)$. Keeping the source's incorrect quadratic sign would reverse the Fourier coordinate. These overall-normalization conventions do not alter the focal-plane placement, but an unapproximated transverse-dependent denominator would not give an exact [Fourier transform](../../../../fourier-transform-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
