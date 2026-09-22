<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

For each mode in [Cartesian coordinates](../../../../../cartesian-coordinate-system.md), $[a_i,a_j^\dagger]=\delta_{ij}$ and $a_i^\dagger a_i=H_i/(\hbar\omega)-1/2$. Consequently the [two-dimensional isotropic harmonic oscillator](../../../../../two-dimensional-isotropic-harmonic-oscillator.md) has

$$
\boxed{H=\hbar\omega(N_x+N_y+1)},\qquad N_i=a_i^\dagger a_i,\qquad E_{kl}=\hbar\omega(k+l+1).
$$

The normalized actions of the [creation and annihilation operators](../../../../../creation-and-annihilation-operators.md) are

$$
a_x|k,l\rangle=\sqrt{k}\,|k-1,l\rangle,\qquad
a_y^\dagger|k,l\rangle=\sqrt{l+1}\,|k,l+1\rangle,\qquad
a_x|0,l\rangle=0.
$$

Invert their definitions as $x=\sqrt{\hbar/(2m\omega)}(a_x+a_x^\dagger)$ and $p_x=i\sqrt{m\hbar\omega/2}(a_x^\dagger-a_x)$, and similarly for $y$. [linear operators](../../../../../linear-operator.md) belonging to different coordinates commute, so substitution into $L_z=xp_y-yp_x$ gives

$$
L_z=\frac{i\hbar}{2}\big[(a_x+a_x^\dagger)(a_y^\dagger-a_y)-(a_y+a_y^\dagger)(a_x^\dagger-a_x)\big]
=\boxed{-i\hbar(a_x^\dagger a_y-a_y^\dagger a_x)}.
$$

Each term transfers one excitation between the two modes: $[N_x+N_y,a_x^\dagger a_y]=(1-1)a_x^\dagger a_y=0$, and likewise for its adjoint. Thus $[H,L_z]=0$ and, with no explicit time dependence, $dL_z/dt=(i/\hbar)[H,L_z]=0$. This is [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) under [planar rotations](../../../../../planar-rotation.md).

Finally $L_z|1,0\rangle=i\hbar|0,1\rangle$ and $L_z|0,1\rangle=-i\hbar|1,0\rangle$. Hence

$$
\boxed{L_z\big(|1,0\rangle+i|0,1\rangle\big)
=\hbar\big(|1,0\rangle+i|0,1\rangle\big)}.
$$

The [angular momentum](../../../../../angular-momentum.md) is $+\hbar$; division by $\sqrt2$ performs [wavefunction normalization](../../../../../wavefunction-normalization.md) on this state without changing its [eigenvalue](../../../../../eigenvalue.md). It is one excitation of the positive circular mode.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
