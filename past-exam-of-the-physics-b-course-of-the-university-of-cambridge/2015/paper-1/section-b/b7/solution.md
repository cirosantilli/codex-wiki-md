<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

The differential form of [Faraday's law of induction](../../../../../faraday-s-law-of-induction.md) is

$$
\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t}.
$$

By [Stokes theorem](../../../../../stokes-theorem.md), for a stationary oriented circuit it becomes $\mathcal E=\oint\mathbf E\cdot d\boldsymbol\ell=-d\Phi_B/dt$, where $\Phi_B=\int\mathbf B\cdot d\mathbf S$ is [magnetic flux](../../../../../magnetic-flux.md) and $\mathcal E$ is [electromotive force](../../../../../electromotive-force.md). Circuit orientation and surface normal obey the [right-hand rule](../../../../../right-hand-rule.md). [Lenz's law](../../../../../lenz-s-law.md) is the physical meaning of the minus sign: the induced current's [magnetic field](../../../../../magnetic-field-split.md) opposes the change in linked [magnetic flux](../../../../../magnetic-flux.md). For a moving circuit, the force per unit [electric charge](../../../../../electric-charge-split.md) is $\mathbf E+\mathbf v\times\mathbf B$, and its line integral is the corresponding [electromotive force](../../../../../electromotive-force.md). Motion through a static [magnetic field](../../../../../magnetic-field-split.md) can therefore induce a [voltage](../../../../../voltage.md) even when $\partial_t\mathbf B=0$.

Let $\theta$ be the wire's angle from the downward vertical, $r=L\sin\theta$, and choose $\boldsymbol\omega$ and $\mathbf B$ upward, as in the figure. The motional term along the wire has radial component $B\omega s$ at cylindrical radius $s$. In steady electrical [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), integrating from the grounded axis to the bob gives

$$
V_b=\int_0^rB\omega s\,ds=\frac12B\omega r^2,
\qquad Q=CV_b=\frac12BC\omega r^2.
$$

The [Lorentz force](../../../../../lorentz-force.md) on this positive [electric charge](../../../../../electric-charge-split.md) is radially outward. Its ratio to the required centripetal term is $QB/(m\omega)\lesssim CB^2L^2/(2m)$, so the stated heavy-bob condition makes its effect on the zero-field [conical pendulum](../../../../../conical-pendulum.md) geometry negligible. With wire tension $T_w$, $T_w\cos\theta=mg$ and $T_w\sin\theta=m\omega^2r$, giving $\cos\theta=g/(\omega^2L)$. Hence the [magnetically charged conical pendulum](../../../../../magnetically-charged-conical-pendulum.md) has

$$
\boxed{Q_0=\frac12BC\left(\omega L^2-\frac{g^2}{\omega^3}\right).}
$$

A nonzero-radius orbit requires $\omega^2L>g$. Reversing the sense of rotation or the [magnetic field](../../../../../magnetic-field-split.md) reverses the sign of $Q_0$.

The response to the added [electric field](../../../../../electric-field-split.md) requires an electrical convention. In the usual mechanical approximation, treat the pre-existing [electric charge](../../../../../electric-charge-split.md) as $Q_0$, include its upward [electric force](../../../../../electric-force.md) $Q_0E$, and neglect all magnetic-force feedback. Then

$$
\cos\theta(E)=\frac{mg-Q_0E}{m\omega^2L},\qquad
\frac{\delta r}{r}=-\frac{\cos\theta\,\delta(\cos\theta)}{\sin^2\theta}
=\frac{Q_0E g}{m\omega^4r^2}
=\boxed{\frac{CBgE}{2m\omega^3}.}
$$

This predicts an increased radius for $Q_0E>0$. It is the result when the newly applied field is used only as a probe force on the original [electric charge](../../../../../electric-charge-split.md).

There is a first-order qualification if the bob remains electrically connected to the grounded pivot and the uniform added field's potential is included consistently. Put $s=\cos\theta$ and set the external [electric potential](../../../../../electric-potential.md) to zero at the pivot. The external potential at the bob is then $ELs$, so the charging relation and full force balance become

$$
Q=C\!\left[\frac12B\omega L^2(1-s^2)-ELs\right],\qquad
\omega^2Ls+\frac Qm(B\omega Ls+E)=g.
$$

The second equation follows by eliminating the wire tension between vertical balance and radial balance, including the outward magnetic [Lorentz force](../../../../../lorentz-force.md). Expanding both equations to first order in $E$, and to leading order in $CB^2L^2/m$, with $s_0=g/(\omega^2L)$, gives

$$
\delta s=-\frac{CBLE}{2m\omega}(1-3s_0^2),\qquad
\boxed{\frac{\delta r}{r}=\frac{CBgE}{2m\omega^3}\,
\frac{1-3s_0^2}{1-s_0^2}.}
$$

The extra factor arises from the added field changing $Q$ by $-CELs_0$ and therefore changing the radial magnetic [force](../../../../../force-split.md). That term is linear in $E$ too; the heavy-bob assumption alone does not justify retaining $Q_0E$ while dropping it. The two expressions refer to the two electrical approximations just specified. The expansion requires a small change relative to the initial radius and is nonuniform as that radius tends to zero.

For an electrical measurement, route the grounded connection through a sensitive [electrometer](../../../../../electrometer.md) operated near zero input [voltage](../../../../../voltage.md), and integrate the charging [electric current](../../../../../electric-current.md) when $B$ or $\omega$ is changed. Starting with the field off, the transferred [electric charge](../../../../../electric-charge-split.md) is $Q_0$ in this ideal capacitance model. Reversing $B$ separates the induced signal from offsets. Alternatively, isolate the charged bob briefly and measure its [electric potential](../../../../../electric-potential.md) with a high-input-impedance [electrometer](../../../../../electrometer.md), accounting for the instrument's extra [capacitance](../../../../../capacitance.md) and for the fact that isolation changes the electrical boundary condition.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
