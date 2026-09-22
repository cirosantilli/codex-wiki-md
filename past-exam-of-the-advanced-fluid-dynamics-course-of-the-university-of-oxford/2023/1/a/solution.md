<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the inviscid limit of the [Navier-Stokes equation](../../../../navier-stokes-equation.md), neglect gravity, and use [ideal magnetohydrodynamics](../../../../ideal-magnetohydrodynamics-split.md). The governing equations are

$$
\nabla\cdot\mathbf v=0,\qquad
\rho(\partial_t\mathbf v+\mathbf v\cdot\nabla\mathbf v)=-\nabla P+\frac{(\nabla\times\mathbf B)\times\mathbf B}{\mu_0},\qquad
\partial_t\mathbf B=\nabla\times(\mathbf v\times\mathbf B),\quad\nabla\cdot\mathbf B=0.
$$

The [continuity equation](../../../../continuity-equation.md) also gives $D_t\rho=0$. Write the first-order magnetic perturbation as $\mathbf b=\mathbf B'$ and linearize about the uniform stationary background:

$$
\rho_0\partial_t\mathbf v=-\nabla\left(P'+\frac{B_0b_z}{\mu_0}\right)+\frac{B_0}{\mu_0}\partial_z\mathbf b,
\qquad\partial_t\mathbf b=B_0\partial_z\mathbf v,
\qquad\nabla\cdot\mathbf v=\nabla\cdot\mathbf b=0.
$$

For a nonzero-[wavenumber](../../../../wavenumber.md) [plane wave](../../../../plane-wave.md) proportional to $e^{i(kz-\omega t)}$, the two divergence constraints imply $v_z=b_z=0$. The longitudinal momentum equation then gives $P'=0$ for that mode, and $\partial_t\rho'=0$ gives $\rho'=0$ for nonzero $\omega$. Thus the propagating [Alfvén wave](../../../../alfven-wave.md) is transverse. Its two independent transverse directions have the same [dispersion relation](../../../../dispersion-relation-split.md).

The [Linear Alfvén wave equations](../../../../linear-alfven-wave-equations.md) reduce to

$$
-i\omega\rho_0\mathbf v=\frac{ikB_0}{\mu_0}\mathbf b,\qquad-i\omega\mathbf b=ikB_0\mathbf v.
$$

Eliminating either [amplitude](../../../../wave-amplitude.md) gives

$$
\boxed{\omega^2=k^2v_A^2,\qquad v_A=\frac{B_0}{\sqrt{\mu_0\rho_0}},\qquad\mathbf b=-\frac{kB_0}{\omega}\mathbf v.}
$$

For $B_0>0$, the branch traveling along $+z$ has $\omega=kv_A$ and $\mathbf b=-\sqrt{\mu_0\rho_0}\mathbf v$. The opposite branch reverses that [amplitude](../../../../wave-amplitude.md) sign. Finite [viscosity](../../../../dynamic-viscosity-split.md) would additionally damp the motion; it is neglected in obtaining the real ideal [dispersion relation](../../../../dispersion-relation-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
