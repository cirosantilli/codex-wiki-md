<h1 id="section-b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

**Powered vertical flight.** Take upward [velocity](../../../../velocity.md) $v$ as positive, and let $v_e>0$ be the downward exhaust [speed](../../../../speed.md) relative to the rocket. During $dt$ the rocket's [mass](../../../../mass.md) changes by $dm<0$, and exhaust mass $-dm$ leaves with Earth-frame [velocity](../../../../velocity.md) $v-v_e$. Compare the [momentum](../../../../momentum-split.md) of the rocket plus this newly expelled exhaust before and after the interval:

$$
(m+dm)(v+dv)+(-dm)(v-v_e)-mv=-mg\,dt.
$$

Discard the second-order product $dm\,dv$. The result is $m\,dv+v_e\,dm=-mg\,dt$, or

$$
m\frac{dv}{dt}=-v_e\frac{dm}{dt}-mg.
$$

The positive [rocket thrust](../../../../rocket-thrust.md) is $-v_e\dot m$. Integrating with $v(0)=0$ and $m(0)=m_0$ gives the [rocket equation](../../../../rocket-equation.md) with gravitational loss:

$$
\boxed{v(t)=v_e\ln\frac{m_0}{m(t)}-gt.}
$$

Using $d(mv)/dt$ for the rocket alone without the exhaust [momentum flux](../../../../momentum-flux.md) would give the wrong equation for this open system.

**Orbital speed under the stated gravity assumption.** A [circular orbit](../../../../circular-orbit.md) of radius $r_o=R_E+h_o=7.90\times10^6\,\mathrm m$ requires [centripetal acceleration](../../../../centripetal-acceleration.md) $v_o^2/r_o$. If the magnitude of [gravitational acceleration](../../../../gravitational-acceleration.md) is the stipulated constant $g=9.8\,\mathrm{m\,s^{-2}}$ even at the orbit,

$$
\frac{v_o^2}{r_o}=g,
\qquad
\boxed{v_o=\sqrt{gr_o}=8.80\times10^3\,\mathrm{m\,s^{-1}}.}
$$

This treats gravity as centrally directed for the orbital calculation, while retaining its constant magnitude. The subsequent flat-surface approximation treats its direction as locally vertical.

**Burnout height.** During the unpowered [projectile motion](../../../../projectile-motion.md), horizontal [velocity](../../../../velocity.md) is constant. At the top of the trajectory the vertical component vanishes, so the horizontal component must equal the orbital [speed](../../../../speed.md) $v_o$. At burnout, therefore,

$$
v_{y,b}=v_o\tan30^\circ,\qquad
h_o-h_b=\frac{v_{y,b}^2}{2g}=\frac{v_o^2}{6g}.
$$

These follow either by integrating $\ddot y=-g$ or by the vertical [work-energy theorem](../../../../work-energy-theorem.md). Substituting the preceding constant-$g$ orbital result gives

$$
\boxed{h_b=h_o-\frac{R_E+h_o}{6}
=1.83\times10^5\,\mathrm m\simeq183\,\mathrm{km}.}
$$

The vertical component is initially positive, as required to reach the orbit after burnout.

**Alternative inverse-square interpretation.** A real Earth's exterior [Newtonian gravitational field](../../../../newtonian-gravitational-field.md) is not constant over a $1500\,\mathrm{km}$ altitude change. If $9.8\,\mathrm{m\,s^{-2}}$ instead means the surface value $g_0$, then [Newton's law of universal gravitation](../../../../newton-s-law-of-universal-gravitation-split.md) gives $GM=g_0R_E^2$ and

$$
v_o=\sqrt{\frac{g_0R_E^2}{R_E+h_o}}=7.13\times10^3\,\mathrm{m\,s^{-1}}.
$$

Using this orbital [speed](../../../../speed.md) but the paper's constant-$g$ flat [projectile motion](../../../../projectile-motion.md) approximation for the coast would give

$$
\boxed{h_b=1.50\times10^6-
\frac{R_E^2}{6(R_E+h_o)}=6.36\times10^5\,\mathrm m\simeq636\,\mathrm{km}.}
$$

This alternative changes the global constant-gravity assumption; it is not the same model as the $183\,\mathrm{km}$ result. An exact curved [Kepler orbit](../../../../kepler-orbit.md) coast would also abandon the prescribed flat trajectory. The printed assumptions support the constant-magnitude answers above, while the inverse-square values explain the different answer obtained from the usual physical Earth-orbit formula.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
