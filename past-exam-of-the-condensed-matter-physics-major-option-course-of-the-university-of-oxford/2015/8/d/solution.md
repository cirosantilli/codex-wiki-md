<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [AC Josephson effect](../../../../ac-josephson-effect.md) is $V=(\Phi_0/2\pi)\dot\delta$. Since the imposed flux is held fixed when defining a small-signal [inductance](../../../../inductance.md), differentiate [c](../c.md) to obtain

$$
\dot I=2I_C\cos\phi\cos\delta\,\dot\delta,\qquad
\boxed{L(\delta,\Phi)=\frac{V}{\dot I}
=\frac{\Phi_0}{4\pi I_C\cos\phi\cos\delta}.}
$$

On the stable small-current branch with $\cos\phi>0$, $\delta\simeq0$ and the result reduces to the printed expression,

$$
\boxed{L_{\rm eff}=\frac{\Phi_0}{4\pi I_C\cos(\pi\Phi/\Phi_0)}.}
$$

The [stable small-signal inductance of a symmetric DC SQUID](../../../../stable-small-signal-inductance-of-a-symmetric-dc-squid.md) requires $|I|\ll2I_C|\cos\phi|$, stronger than $I\ll I_C$ near a half-integer flux quantum. If $\cos\phi<0$, the stable zero-current phase is $\delta\simeq\pi$ and $\cos\delta\simeq-1$. Its [inductance](../../../../inductance.md) is positive:

$$
\boxed{L_{\rm stable}=\frac{\Phi_0}{4\pi I_C|\cos(\pi\Phi/\Phi_0)|}.}
$$

For example, $\Phi=\Phi_0$ makes the printed signed formula negative when expanded about $\delta=0$, but that phase is an energy maximum. Expanding about the stable $\delta=\pi$ corrects the sign. At ideal half-integer flux the critical current vanishes and the linear [inductance](../../../../inductance.md) formally diverges; a finite transport current cannot satisfy the small-current approximation there. Geometric [inductance](../../../../inductance.md) and other nonidealities then have to be retained instead of extending the simple formula through its pole.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
