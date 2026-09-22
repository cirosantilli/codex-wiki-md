<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $\chi=kx-\omega t$, with $k>0$. The [surface elevation](../../../../../surface-elevation.md) is $\eta=\alpha\cos\chi$, so $\eta_t=\alpha\omega\sin\chi$. Use [separation of variables](../../../../../separation-of-variables.md) in the interior [Laplace equation](../../../../../laplace-equation.md):

$$
\phi=A\cosh(k(z+h))\sin\chi.
$$

The $\sinh(k(z+h))$ term is excluded by the bed [no-penetration boundary condition](../../../../../no-penetration-boundary-condition.md). The linear surface [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) determines

$$
Ak\sinh(kh)=\alpha\omega,
\qquad
\boxed{\phi(x,z,t)=\frac{\alpha\omega}{k\sinh(kh)}
\cosh(k(z+h))\sin(kx-\omega t)}.
$$

An irrelevant additive constant is omitted. At $z=0$,

$$
\phi_t=-\frac{\alpha\omega^2}{k}\coth(kh)\cos\chi,
\qquad \eta_{xxxx}=\alpha k^4\cos\chi.
$$

The linear dynamic boundary condition then reduces to

$$
-\frac{\omega^2}{k}\coth(kh)+g+\frac B\rho k^4=0.
$$

Consequently the [dispersion relation of a floating elastic plate](../../../../../dispersion-relation-of-a-floating-elastic-plate.md) with zero plate inertia is

$$
\boxed{\omega^2=\left(gk+\frac B\rho k^5\right)\tanh(kh),\qquad
\omega(k)=\sqrt{\left(gk+\frac B\rho k^5\right)\tanh(kh)}}.
$$

The negative-frequency branch gives propagation in the opposite direction. For signed [wavenumber](../../../../../wavenumber.md), replace $k$ by $|k|$ in the squared-frequency formula. Setting $B=0$ recovers the finite-depth [surface gravity wave](../../../../../surface-gravity-wave.md) relation, a useful sign check.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
