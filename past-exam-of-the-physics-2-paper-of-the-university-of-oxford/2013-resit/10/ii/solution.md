<h1 id="10/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The source figure has a series capacitor followed by $R$ in parallel with $L$. Its [complex impedance](../../../../electrical-impedance.md) is

$$
Z=-\frac{i}{\omega C}+\frac{i\omega LR}{R+i\omega L}
=\frac{R\omega^2L^2}{R^2+\omega^2L^2}+i\left[\frac{\omega LR^2}{R^2+\omega^2L^2}-\frac1{\omega C}\right].
$$

The imaginary part vanishes at a finite positive frequency only if $R^2C>L$, in which case

$$
\boxed{\omega_*^2=\frac{R^2}{L(R^2C-L)}=\frac1{LC-L^2/R^2}.}
$$

At that frequency, substituting $R^2+\omega_*^2L^2=\omega_*^2LR^2C$ into the real part gives

$$
\boxed{Z(\omega_*)=\frac{L}{RC}.}
$$

If $R^2C\le L$, no finite positive-frequency cancellation exists; the impedance merely tends toward its high-frequency limit.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [10](../../10.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
