<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use $\phi_j=U_jx-\tfrac12U_j^2t+\phi'_j$ and retain terms linear in the displacement and perturbation potentials. Evaluation at $z=\eta$ may then be replaced by evaluation at $z=0$: the correction to a perturbation is second order. The [kinematic boundary conditions](../../../../../../../kinematic-boundary-condition.md) become

$$
\partial_z\phi'_j=(\partial_t+U_j\partial_x)\eta\quad(z=0).
$$

The linearized [pressure continuity](../../../../../../../pressure-continuity.md) is

$$
\rho_1(\partial_t+U_1\partial_x)\phi'_1
-\rho_2(\partial_t+U_2\partial_x)\phi'_2
+g(\rho_1-\rho_2)\eta=0.
$$

The decaying [normal modes](../../../../../../../normal-mode.md) give $-kA_1=ik(U_1-c)B$ and $kA_2=ik(U_2-c)B$. Thus $A_1=-i(U_1-c)B$, $A_2=i(U_2-c)B$. Substitution into the dynamic condition yields the [Kelvin-Helmholtz dispersion relation with gravity](../../../../../../../kelvin-helmholtz-dispersion-relation-with-gravity.md),

$$
\rho_1(U_1-c)^2+\rho_2(U_2-c)^2=\frac{g(\rho_2-\rho_1)}k.
$$

Put $\rho=\rho_1+\rho_2$ and $\overline U=(\rho_1U_1+\rho_2U_2)/\rho$. [Completing the square](../../../../../../../completing-the-square.md) gives

$$
c=\overline U\pm\sqrt{\frac{g(\rho_2-\rho_1)}{\rho k}
-\frac{\rho_1\rho_2(U_1-U_2)^2}{\rho^2}}.
$$

For $k>0$, the [temporal growth rate](../../../../../../../growth-rate.md) is $kc_i$. A growing [complex conjugate](../../../../../../../complex-conjugate.md) branch therefore exists precisely when the radicand of the [square root](../../../../../../../square-root.md) is negative:

$$
\boxed{k>\frac{g(\rho_2^2-\rho_1^2)}{\rho_1\rho_2(U_1-U_2)^2}.}
$$

At equality the two [phase velocities](../../../../../../../phase-velocity.md) coincide and there is no exponential growth. Below it the roots describe real [internal gravity waves](../../../../../../../internal-wave.md). The denser lower fluid gives stable [density stratification](../../../../../../../density-stratification.md), but the tangential shear can overcome it. The assumption $U_1\ne U_2$ is needed for the displayed threshold; equal streams have no such shear instability.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
