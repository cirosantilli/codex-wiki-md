<h1 id="section-b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For particles in an [inertial frame](../../../../inertial-frame.md), total [momentum](../../../../momentum-split.md) and [angular momentum](../../../../angular-momentum.md) about a fixed origin are

$$
\boxed{\mathbf P=\sum_i m_i\mathbf v_i,\qquad \mathbf L_O=\sum_i\mathbf r_i\times m_i\mathbf v_i.}
$$

The [momentum](../../../../momentum-split.md) derivative is the total external [force](../../../../force-split.md) when internal forces cancel pairwise. [Angular momentum](../../../../angular-momentum.md) is conserved when the total external [torque](../../../../torque.md) vanishes and the internal torques sum to zero, as for pairwise equal-and-opposite central forces. Equal-and-opposite internal forces alone need not cancel internal [torque](../../../../torque.md) if their lines of action are different. An isolated system with these internal-[force](../../../../force-split.md) properties conserves both quantities; if fields carry [momentum](../../../../momentum-split.md), the complete system must include them.

For a straight rocket, let its instantaneous remaining [mass](../../../../mass.md) be $M$ and let $dM<0$ be ejected during a [velocity](../../../../velocity.md) increase $dv$. The exhaust's inertial [velocity](../../../../velocity.md) is $v-v_e$ to first order. [Conservation of momentum](../../../../momentum-conservation.md) gives

$$
Mv=(M+dM)(v+dv)+(-dM)(v-v_e),\qquad M\,dv=-v_e\,dM.
$$

Integrating from initial [mass](../../../../mass.md) $m+m_f$ to dry [mass](../../../../mass.md) $m$ yields the [rocket equation](../../../../rocket-equation.md)

$$
\boxed{v=v_e\log\frac{m+m_f}{m}.}
$$

It is the rocket-plus-exhaust system that is isolated; the rocket alone is a variable-[mass](../../../../mass.md) open system.

For the firework, the original diagram places one tangentially firing point rocket at the end of each radial rod. The [parallel axis theorem](../../../../parallel-axis-theorem.md) changes each rod's central inertia to $ma^2/12+m(a/2)^2=ma^2/3$. Adding all rods and fueled rockets gives

$$
\boxed{I_i=3\left[\frac{ma^2}{3}+(m+m_f)a^2\right]=(4m+3m_f)a^2.}
$$

When fuel is exhausted, $I_f=4ma^2$.

Let $M_f$ now denote the total remaining fuel in all three rockets, so $I=4ma^2+a^2M_f$. Fuel at the rim co-rotates before ejection. Its backward tangential exhaust [velocity](../../../../velocity.md) is $a\omega-v_e$, and its [angular momentum](../../../../angular-momentum.md) per unit [mass](../../../../mass.md) about the axle is $a(a\omega-v_e)$. For an infinitesimal ejection,

$$
I\omega=(I+dI)(\omega+d\omega)+(-dM_f)a(a\omega-v_e).
$$

Since $dI=a^2dM_f$, the co-rotation terms cancel and leave $I\,d\omega=-av_e\,dM_f$. The [tangential-exhaust rotor with a fixed dry inertia](../../../../tangential-exhaust-rotor-with-a-fixed-dry-inertia.md) therefore obeys

$$
\omega_f=\frac{v_e}{a}\log\frac{I_i}{I_f},\qquad \boxed{\omega_f=\frac{v_e}{a}\log\beta,\quad \beta=\frac{4m+3m_f}{4m}=1+\frac{3m_f}{4m}.}
$$

Neglecting the exhaust's initial tangential motion would give an incorrect angular-[momentum](../../../../momentum-split.md) balance. The rod [mass](../../../../mass.md) remains in the denominator throughout the burn.

After the burn, the opposing constant axle [torque](../../../../torque.md) $G>0$ acts on the fixed inertia $I_f$. Its [work](../../../../work.md) over the remaining turn equals the initial [rotational kinetic energy](../../../../rotational-kinetic-energy.md):

$$
G\Delta\theta=\frac12I_f\omega_f^2,\qquad \boxed{\Delta\theta=\frac{2ma^2\omega_f^2}{G}=\frac{2mv_e^2}{G}(\log\beta)^2.}
$$

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Section B](../../section-b.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
