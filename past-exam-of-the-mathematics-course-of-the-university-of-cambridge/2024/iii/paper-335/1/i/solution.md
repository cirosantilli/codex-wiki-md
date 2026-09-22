<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define

$$
A=\partial_x,
\qquad
B=\left(n^2+k_0^{-2}\partial_z^2\right)^{1/2}.
$$

If $A$ and $B$ commute, the [Helmholtz equation](../../../../../../helmholtz-equation.md) operator factorizes as

$$
A^2+k_0^2B^2
=(A+ik_0B)(A-ik_0B).
$$

When $n$ varies with $x$, the exact product also contains the [commutator](../../../../../../commutator.md) $[A,B]$; neglecting it assumes longitudinal changes are slow. The forward-propagating factor is

$$
(A-ik_0B)\psi=0,
$$

because it admits $e^{ik_0x}$ in a uniform medium.

Put $\psi=Ee^{ik_0x}$. The one-way equation becomes

$$
E_x=ik_0(B-1)E.
$$

For

$$
Q=n^2-1+k_0^{-2}\partial_z^2,
$$

the [Taylor expansion](../../../../../../taylor-expansion.md) $(1+Q)^{1/2}=1+Q/2+O(Q^2)$ gives

$$
E_x=\frac{i}{2k_0}E_{zz}
+\frac{ik_0}{2}(n^2-1)E.
$$

Thus the [parabolic wave equation](../../../../../../parabolic-wave-equation.md) is

$$
\boxed{
2ik_0E_x+E_{zz}
+k_0^2(n^2-1)E=0}.
$$

The expansion is accurate under the [paraxial approximation](../../../../../../paraxial-approximation.md): transverse wavenumbers satisfy $|k_z|/k_0\ll1$, the envelope varies slowly on the carrier scale, the refractive-index contrast is weak enough for $Q^2$ to be negligible, and $n$ varies slowly in $x$ so $[A,B]$ is small. The one-way factor discards backward propagation and reflection; the square-root expansion additionally discards large-angle and higher-order diffraction, and it does not accurately represent strongly evanescent components or abrupt longitudinal interfaces.

## ↑ Ancestors (11)

1. [I](../i.md)
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
