<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At $t=0$ the [power series](../../../../power-series.md) gives $\mathbf v(0)=\mathbf v_0$. Equate the coefficient of $t^n$ after differentiating the series and substituting into the [linear system of ordinary differential equations](../../../../linear-system-of-differential-equations.md):

$$
(n+1)\mathbf v_{n+1}=-iH\mathbf v_n.
$$

[Mathematical induction](../../../../mathematical-induction.md) yields $\mathbf v_n=(-iH)^n\mathbf v_0/n!$. Summing gives the [matrix exponential](../../../../matrix-exponential.md) solution $\mathbf v(t)=e^{-iHt}\mathbf v_0$.

For the specified diagonal [Hermitian matrix](../../../../hermitian-operator.md), its powers and exponential act separately on the two components. Thus

$$
\boxed{U(t)=e^{-iHt}=\begin{pmatrix}e^{-it}&0\\0&e^{it}\end{pmatrix},\qquad\mathbf v(t)=U(t)\mathbf v_0.}
$$

This [unitary matrix](../../../../unitary-matrix.md) preserves $\mathbf v^\dagger\mathbf v$: the two components acquire opposite phases of unit [modulus](../../../../modulus.md). The coefficient recurrence applies to any constant finite square matrix $H$; unitarity here additionally uses its [Hermitian](../../../../hermitian-operator.md) property.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
