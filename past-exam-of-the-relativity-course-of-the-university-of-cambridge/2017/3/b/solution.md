<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the [inertial frame](../../../../inertial-frame.md) $S'$ move at speed $v$ in the positive $x$ direction relative to $S$, with parallel axes and coincident origins at zero time. The inverse [Lorentz transformation](../../../../lorentz-transformation.md) gives

$$
dt=\gamma_v(dt'+v\,dx'/c^2),\quad dx=\gamma_v(dx'+v\,dt'),\quad dy=dy',\quad dz=dz'.
$$

Here $\gamma_v=(1-v^2/c^2)^{-1/2}$ and $\mathbf u'=d\mathbf x'/dt'$ is the particle's [velocity](../../../../velocity.md) in $S'$. Dividing spatial differentials by $dt$ gives the [relativistic velocity addition](../../../../velocity-addition-formula.md) law

$$
\boxed{u_x=\frac{u_x'+v}{1+vu_x'/c^2},\qquad
u_y=\frac{u_y'}{\gamma_v(1+vu_x'/c^2)},\qquad
u_z=\frac{u_z'}{\gamma_v(1+vu_x'/c^2)}.}
$$

For the collision, set $c=1$ during the algebra. Let the incident projectile have [energy](../../../../energy-split.md) $E>m_1$ and [momentum](../../../../momentum-split.md) $p=\sqrt{E^2-m_1^2}$. The target is initially at rest. The squared [invariant mass](../../../../invariant-mass.md), boost speed and [Lorentz factor](../../../../lorentz-factor.md) of the [center-of-momentum frame](../../../../center-of-momentum-frame.md) are

$$
s=m_1^2+m_2^2+2m_2E,\qquad V=\frac p{E+m_2},\qquad\Gamma=\frac{E+m_2}{\sqrt s}.
$$

In that frame the projectile has $p_*=m_2p/\sqrt s$ and $E_*=(m_1^2+m_2E)/\sqrt s$. An [elastic collision](../../../../elastic-collision.md) changes the direction of its [momentum](../../../../momentum-split.md), through an angle $\varphi$, while preserving these magnitudes. Transforming the outgoing [four-momentum](../../../../four-momentum.md) back to the laboratory gives

$$
\tan\theta=\frac{\sin\varphi}{\Gamma(\cos\varphi+B)},\qquad
B=\frac{VE_*}{p_*}=\frac{m_1^2+m_2E}{m_2(E+m_2)}>1.
$$

The maximum occurs at $\cos\varphi=-1/B$. Since

$$
\Gamma^2(B^2-1)=\frac{m_1^2-m_2^2}{m_2^2},
$$

the [maximum laboratory deflection in relativistic elastic scattering](../../../../maximum-laboratory-deflection-in-relativistic-elastic-scattering.md) is

$$
\boxed{\tan\theta_{\max}=\frac{m_2}{\sqrt{m_1^2-m_2^2}},\qquad
\sin\theta\leq\sin\theta_{\max}=\frac{m_2}{m_1}.}
$$

The printed strict inequality needs correction: equality is kinematically attainable. For example, in $c=1$ units take $m_1=2$, $m_2=1$, and incident $E=3$. A projectile scattered through $30^\circ$ with final [energy](../../../../energy-split.md) $16/7$ has [momentum](../../../../momentum-split.md) $(3\sqrt5/7,\sqrt{15}/7)$. The target then has [energy](../../../../energy-split.md) $12/7$ and [momentum](../../../../momentum-split.md) $(4\sqrt5/7,-\sqrt{15}/7)$; both outgoing particles satisfy their [mass shells](../../../../mass-shell.md) and conserve total [four-momentum](../../../../four-momentum.md). This gives $\sin\theta=1/2=m_2/m_1$ exactly. The inequality is strict only away from the maximizing direction.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
