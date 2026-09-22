<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

The quadratic [first integrals](../../../../../first-integral.md) of the torque-free [Euler equations for a torque-free rigid body](../../../../../euler-equations-for-a-torque-free-rigid-body.md) are

$$
\boxed{2E=I_1\omega_1^2+I_2\omega_2^2+I_3\omega_3^2,\qquad
L^2=I_1^2\omega_1^2+I_2^2\omega_2^2+I_3^2\omega_3^2.}
$$

[Differentiation](../../../../../differentiation.md) and substitution of all three Euler equations make each [derivative](../../../../../derivative.md) vanish: the coefficients respectively sum to $(I_2-I_3)+(I_3-I_1)+(I_1-I_2)=0$ and $I_1(I_2-I_3)+I_2(I_3-I_1)+I_3(I_1-I_2)=0$. At either endpoint these constants are $2E=I_2\Omega^2$, $L^2=I_2^2\Omega^2$, proving $L^2=2EI_2$.

Eliminating the other squared components gives, with $s=\omega_2/\Omega$,

$$
\omega_1^2=\frac{I_2(I_3-I_2)}{I_1(I_3-I_1)}\Omega^2(1-s^2),\qquad
\omega_3^2=\frac{I_2(I_2-I_1)}{I_3(I_3-I_1)}\Omega^2(1-s^2).
$$

Hence $|s|\le1$ and the second Euler equation gives $ds/d\tau=\pm(1-s^2)$, where $\tau=\Omega t\sqrt{(I_2-I_1)(I_3-I_2)/(I_1I_3)}$ increases with $t$. The specified orbit goes from $s=1$ to $s=-1$, so its sign must be negative. The sign in the original PDF's reduced equation is therefore inconsistent with its endpoint conditions. The corrected heteroclinic satisfies

$$
\boxed{\frac{ds}{d\tau}=s^2-1,\qquad s(\tau)=-\tanh(\tau-\tau_0).}
$$

Integrating by separation gives this family for $|s|<1$; the integration constant is a time translation. The printed positive-sign equation instead has the increasing solutions $s=\tanh(\tau-\tau_0)$ and cannot meet the stated endpoints. For completeness its other real solutions are $s=\pm1$ and the branches $s=\coth(\tau-\tau_0)$ on intervals avoiding their pole. These latter branches are excluded by the conserved-energy constraint $|s|\le1$. The scalar heteroclinic is unique up to translation. For the full angular-velocity vector there are two sign-related branches: simultaneously reversing $\omega_1$ and $\omega_3$ preserves all three Euler equations and both endpoints. Full-vector uniqueness therefore also requires choosing one of those branches.

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
