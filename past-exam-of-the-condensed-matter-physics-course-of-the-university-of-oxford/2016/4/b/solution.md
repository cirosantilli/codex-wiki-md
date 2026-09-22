<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The right [spring](../../../../spring.md) changes length by $u_{n+1}-u_n$ and pulls [atom](../../../../atom-physics.md) $n$ to the right with [force](../../../../force-split.md) $C(u_{n+1}-u_n)$. The left [spring](../../../../spring.md) contributes $-C(u_n-u_{n-1})$. Adding these [restoring forces](../../../../restoring-force.md) and applying [Newton's second law](../../../../newton-s-second-law.md) gives

$$
m\ddot u_n=C(u_{n+1}-2u_n+u_{n-1}).
$$

Uniform [displacement](../../../../displacement.md) makes both [spring](../../../../spring.md) extensions vanish, as [translational invariance](../../../../translational-symmetry.md) requires. Search for a [normal mode](../../../../normal-mode.md) $u_n=u_0e^{i(kna-\omega t)}$. Substitution yields

$$
-m\omega^2=C(e^{ika}+e^{-ika}-2)=-4C\sin^2(ka/2),
\qquad\boxed{\omega(k)=2\sqrt{C/m}\,|\sin(ka/2)|.}
$$

One representative [first Brillouin zone](../../../../first-brillouin-zone.md) is $-\pi/a\leq k\leq\pi/a$. This is one positive-frequency [acoustic branch](../../../../acoustic-phonon-branch.md): near zero [wavevector](../../../../wavevector.md), $\omega\simeq a\sqrt{C/m}|k|$, so the [sound speed](../../../../speed-of-sound.md) is $v_s=a\sqrt{C/m}$. Opposite signs of $k$ label opposite propagation directions, not a second polarization branch.

The model assumes small [displacements](../../../../displacement.md), [harmonic](../../../../simple-harmonic-motion.md) nearest-neighbor [forces](../../../../force-split.md), one scalar [displacement](../../../../displacement.md) per [atom](../../../../atom-physics.md) and uniform equilibrium spacing. It excludes [damping](../../../../damping.md), [anharmonic](../../../../anharmonicity.md) expansion and transverse polarizations. In a three-dimensional monatomic [crystal](../../../../crystal.md) there would normally be three acoustic polarizations; that counting cannot be imported into this explicitly one-dimensional scalar model.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
