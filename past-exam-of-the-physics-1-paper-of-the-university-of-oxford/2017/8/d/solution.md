<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the sphere's [mass](../../../../mass.md) as $M$ and use $I=2Ma^2/5$ from [b](../b.md). Let $K_n$ and $K_t$ be the upward and rightward contact [impulses](../../../../impulse.md). The initial vertical [velocity](../../../../velocity.md) is $-u_1$ and the outgoing vertical [velocity](../../../../velocity.md) is $u_2$. Perfect normal elasticity gives

$$
u_2=u_1,\qquad K_n=M(u_2+u_1)=2Mu_1.
$$

The tangential and angular [impulse](../../../../impulse.md) equations are

$$
M(v_2-v_1)=K_t,\qquad I(\Omega_2-\Omega_1)=aK_t.
$$

For the ideal [elastic rough-sphere bounce](../../../../elastic-rough-sphere-bounce.md), the tangential translational plus rotational [kinetic energy](../../../../kinetic-energy.md) is restored on separation. Substituting these two equations into that requirement gives

$$
0=K_t(v_1+a\Omega_1)
+\frac{K_t^2}{2}\left(\frac1M+\frac{a^2}{I}\right).
$$

The interacting rough-contact branch, rather than the smooth branch $K_t=0$, therefore has

$$
K_t=-\frac{2(v_1+a\Omega_1)}{1/M+a^2/I}
=-\frac47M(v_1+a\Omega_1).
$$

Consequently, with all tangential quantities signed in the convention of [c](../c.md),

$$
\boxed{u_2=u_1,\qquad
v_2=\frac{3v_1-4a\Omega_1}{7},\qquad
\Omega_2=-\frac{10v_1+3a\Omega_1}{7a}.}
$$

In particular, $v_2+a\Omega_2=-(v_1+a\Omega_1)$: the tangential [contact-point velocity](../../../../contact-point-velocity.md) reverses. The outgoing $v_2$ may be negative; the sphere rebounds backward when $a\Omega_1>3v_1/4$. Substitution also checks both total [kinetic energy](../../../../kinetic-energy.md) and [angular momentum](../../../../angular-momentum.md) about the contact point, $I\Omega-Mav$.

This result uses the conventional perfectly elastic, fully rough contact idealization. The word _rough_ alone, with an unspecified finite [coefficient of friction](../../../../coefficient-of-friction.md), would not determine the outgoing tangential state. For example, imposing sticking at separation would instead give $K_t=-2M(v_1+a\Omega_1)/7$ and dissipate $M(v_1+a\Omega_1)^2/7$, contradicting total elasticity unless $w_1=0$. The displayed elastic branch requires enough tangential [impulse](../../../../impulse.md); a Coulomb bound $|K_t|\leq\mu K_n$ would at least require $\mu\geq2|v_1+a\Omega_1|/(7u_1)$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
