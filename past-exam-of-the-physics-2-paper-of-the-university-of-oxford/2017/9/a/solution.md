<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a current element $I\,d\boldsymbol\ell$, the [Biot-Savart law](../../../../biot-savart-law.md) is

$$
d\mathbf B=\frac{\mu_0I}{4\pi}\frac{d\boldsymbol\ell\times\mathbf R}{R^3}.
$$

Take a straight wire along $z$, extending from $-a$ to $a$, and observe its [magnetic field](../../../../magnetic-field-split.md) at $(s,0,0)$. All contributions point in $+\hat{\boldsymbol\phi}$ for positive $I$ along $+z$, by the [right-hand rule](../../../../right-hand-rule.md). Their magnitude integrates to

$$
B_\phi=\frac{\mu_0I}{4\pi}\int_{-a}^{a}\frac{s\,dz}{(s^2+z^2)^{3/2}}
=\frac{\mu_0I}{4\pi}\left[\frac{z}{s\sqrt{s^2+z^2}}\right]_{-a}^{a}
=\boxed{\frac{\mu_0Ia}{2\pi s\sqrt{s^2+a^2}}}.
$$

For $a/s\to\infty$ this becomes $\mu_0I/(2\pi s)$, so $\oint\mathbf B\cdot d\boldsymbol\ell=2\pi sB_\phi=\mu_0I$, exactly as [Ampère's law](../../../../ampere-s-circuital-law.md) requires for an infinite straight wire.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
