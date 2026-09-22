<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With

$$
D=\frac{i}{2k_0}\partial_z^2,
\qquad
S=\frac{ik_0}{2}(n^2-1),
$$

the [parabolic wave equation](../../../../../../parabolic-wave-equation.md) is $E_x=(D+S)E$. Freeze $S$ at $x_0$, or preferably at the step midpoint. Over a short distance $\Delta x$, [Lie-Trotter splitting](../../../../../../lie-product-formula.md) gives

$$
\boxed{
E(x_0+\Delta x)
\simeq e^{\Delta xD}e^{\Delta xS_0}E(x_0)}.
$$

The reversed ordering has the same first-order accuracy, while symmetric half-steps in $S$ give the more accurate Strang form.

The [commutator](../../../../../../commutator.md) can be displayed explicitly. If $q=n^2-1$, then

$$
[D,S]E
=-\frac14\left(q_{zz}E+2q_zE_z\right).
$$

The splitting assumption requires $\Delta x^2[D,S]E$ to be small relative to $E$. It is favored by a short range step, a transversely smooth refractive index, and a field without unresolved large transverse wavenumbers. Freezing $S$ also requires $\Delta x\,S_x$ to be small. These conditions supplement the one-way and [paraxial approximation](../../../../../../paraxial-approximation.md) already used in part i.

The phase-screen substep is pointwise:

$$
e^{\Delta xS_0}E(x_0,z)
=\exp\left[
\frac{ik_0\Delta x}{2}
(n^2(x_0,z)-1)
\right]E(x_0,z).
$$

Define

$$
\boxed{
\widetilde E_0(x_0,z)
=e^{\Delta xS_0}E(x_0,z)}.
$$

Then solve the free-diffraction initial-value problem

$$
E_x=DE,
\qquad
E(x_0,z)=\widetilde E_0(x_0,z),
$$

to $x_0+\Delta x$. In transverse [Fourier transform](../../../../../../fourier-transform.md) variables, this substep is simply

$$
\widehat E(x_0+\Delta x,k_z)
=e^{-ik_z^2\Delta x/(2k_0)}
\widehat{\widetilde E}_0(k_z).
$$

This is the [split-step Fourier method](../../../../../../split-step-fourier-method.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
