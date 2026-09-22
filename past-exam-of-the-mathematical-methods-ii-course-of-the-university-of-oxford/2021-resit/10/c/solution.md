<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [reflection of a string wave from a freely moving endpoint mass](../../../../reflection-of-a-string-wave-from-a-freely-moving-endpoint-mass.md), let $c=\sqrt{T/\mu}$, $k=\omega/c>0$ and use the complex [time-harmonic wave](../../../../time-harmonic-wave.md) convention

$$
y(x,t)=\operatorname{Re}\left\{A_i\left(e^{ikx}+R e^{-ikx}\right)e^{-i\omega t}\right\},
\qquad x\le0.
$$

The string pulls its endpoint toward negative $x$, so its transverse [force](../../../../force-split.md) on the attached [mass](../../../../mass.md) is $-Ty_x(0,t)$. [Newton's second law](../../../../newton-s-second-law.md) gives the [boundary condition](../../../../boundary-condition.md) $my_{tt}(0,t)=-Ty_x(0,t)$. Substitution yields

$$
m\omega^2(1+R)=iTk(1-R),\qquad
\boxed{R=\frac{iTk-m\omega^2}{iTk+m\omega^2}
=\frac{Z+i m\omega}{Z-i m\omega},\quad Z=\frac Tc=\sqrt{T\mu}.}
$$

Here $Z$ is the [characteristic impedance of a stretched string](../../../../characteristic-impedance-of-a-stretched-string.md). Since the incident and reflected [waves](../../../../wave-split.md) share the same string, their mean [power](../../../../power.md) ratio is the squared modulus of this displacement [reflection coefficient](../../../../reflection-coefficient.md):

$$
\boxed{\mathcal R=|R|^2=1.}
$$

There is **no remaining fraction of the mean incident energy**: the freely moving [mass](../../../../mass.md) provides no [dissipation](../../../../dissipation.md) and no onward transmission channel. It exchanges [kinetic energy](../../../../kinetic-energy.md) with the string during each cycle but has zero mean absorbed [power](../../../../power.md). Indeed the [energy flux of a transverse string wave](../../../../energy-flux-of-a-transverse-string-wave.md) satisfies

$$
-Ty_xy_t\big|_{x=0}
=my_{tt}y_t
=\frac{d}{dt}\left(\frac12my_t(0,t)^2\right),
$$

whose cycle average is zero. As checks, $m\to0$ gives $R=+1$, the [free-end reflection of a transverse string wave](../../../../free-end-reflection-of-a-transverse-string-wave.md), while $m\to\infty$ at fixed $\omega>0$ gives $R=-1$, the fixed-end limit.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
