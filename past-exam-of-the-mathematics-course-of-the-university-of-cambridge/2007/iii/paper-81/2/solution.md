<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose the helix handedness so its unit tangent is $\mathbf t=\cos\alpha\,\mathbf i+\sin\alpha\,\mathbf e_\phi$. Let $q=\Omega_0-\Omega$; the body rotates at $+\Omega\mathbf i$, while the flagellum rotates at $-q\mathbf i$ in the laboratory, since its relative motor rotation is $-\Omega_0\mathbf i$. Both translate at $-U\mathbf i$. Thus the relative fluid [velocity](../../../../../velocity.md) on a flagellar element is $\mathbf w=U\mathbf i+bq\mathbf e_\phi$.

Low-Reynolds-number [resistive-force theory](../../../../../resistive-force-theory.md) gives [force](../../../../../force.md) per unit length on the flagellum

$$
\mathbf f=K_N\mathbf w+(K_T-K_N)(\mathbf w\cdot\mathbf t)\mathbf t.
$$

Its axial and azimuthal components are

$$
f_x=(K_N\sin^2\alpha+K_T\cos^2\alpha)U-(K_N-K_T)bq\sin\alpha\cos\alpha,
$$



$$
f_\phi=(K_N\cos^2\alpha+K_T\sin^2\alpha)bq-(K_N-K_T)U\sin\alpha\cos\alpha.
$$

Define the integrated [axial resistance matrix of a slender helix](../../../../../axial-resistance-matrix-of-a-slender-helix.md) coefficients

$$
A=L(K_N\sin^2\alpha+K_T\cos^2\alpha),\quad
C=bL(K_N-K_T)\sin\alpha\cos\alpha,\quad
H=b^2L(K_N\cos^2\alpha+K_T\sin^2\alpha).
$$

The sphere has translational resistance $A_b=6\pi\mu a$ by the [Stokes drag law](../../../../../stokes-s-law.md) and rotational resistance $H_b=8\pi\mu a^3$. Its hydrodynamic [force](../../../../../force.md) is $+A_bU\mathbf i$ and its [torque](../../../../../torque.md) $-H_b\Omega\mathbf i$. Integration of $f_x$ and $bf_\phi$ gives the zero total [force](../../../../../force.md) and [torque](../../../../../torque.md) conditions

$$
\boxed{(A+A_b)U=Cq,\qquad CU=Hq-H_b\Omega.}
$$

Dividing the first by $L$ and expanding the coefficients gives exactly the two requested balances. The internal motor [torque](../../../../../torque.md) cancels in the total [torque](../../../../../torque.md) balance; it is not an external applied [torque](../../../../../torque.md).

Eliminate $U$ and use $q+\Omega=\Omega_0$. The effective flagellar rotational resistance is $H_e=H-C^2/(A+A_b)$, so

$$
q=\frac{H_b\Omega_0}{H_b+H_e},\qquad
\boxed{\Omega=\frac{H_e\Omega_0}{H_b+H_e},\qquad
U=\frac{CH_b\Omega_0}{(A+A_b)(H+H_b)-C^2}.}
$$

The [determinant of helical resistance in resistive-force theory](../../../../../determinant-of-helical-resistance-in-resistive-force-theory.md) is $AH-C^2=b^2L^2K_NK_T>0$, hence the denominator is positive. Opposite handedness changes the sign of the translation-rotation coupling and reverses the swimming direction.

For $K_T=K$, $K_N=2K$, $\alpha=\pi/4$ and $a=b$, the coefficients are $A=3KL/2$, $C=KaL/2$, $H=3Ka^2L/2$. Therefore

$$
\boxed{U=\frac{4\pi\mu KL a^2\Omega_0}{2K^2L^2+21\pi\mu aKL+48\pi^2\mu^2a^2}.}
$$

Equivalently, with $h=KL/(\pi\mu a)$, $U=a\Omega_0\,4h/(2h^2+21h+48)$. These are positive speed magnitudes for the selected handedness; the translational [velocity](../../../../../velocity.md) is $-U\mathbf i$.

This [helical microswimmer with a spherical head](../../../../../helical-microswimmer-with-a-spherical-head.md) approximation neglects head-tail hydrodynamic interactions as permitted, treats the flagellum as slender and rigid, and averages away transverse [forces](../../../../../force.md) associated with finite helical ends. The flow is quasistatic [Stokes flow](../../../../../stokes-flow-split.md), so neither body inertia nor fluid inertia enters the balance.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
