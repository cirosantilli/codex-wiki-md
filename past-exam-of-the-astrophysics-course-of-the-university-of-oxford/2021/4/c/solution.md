<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the dimensionally correct flat [Friedmann-Lemaître-Robertson-Walker metric](../../../../friedmann-lemaitre-robertson-walker-metric.md)

$$
ds^2=-c^2dt^2+a^2(t)\left[d\chi^2+\chi^2(d\vartheta^2+\sin^2\vartheta\,d\varphi^2)\right].
$$

The source's $-c\,dt^2$ is missing a factor $c$, and its angular term must mean the unit-sphere line element $d\Omega^2$, not the [solid angle](../../../../solid-angle.md) element $d\Omega=\sin\vartheta\,d\vartheta\,d\varphi$. For example, $c\,dt^2$ has dimensions length times time, while $ds^2$ has dimensions length squared. The corrected convention above removes both ambiguities.

A radial light ray has $ds^2=0$ and $|d\chi|=c|dt|/a$. Thus

$$
\frac{d\chi}{dz}=\frac c{H(z)},\qquad
\chi(z)=\frac c{H_0}\int_0^z\frac{du}{(1+u)^{3/2}}
=\frac{2c}{H_0}\left(1-\frac1{\sqrt{1+z}}\right).
$$

A proper shell volume at emission is $dV_{\rm proper}=a^3\chi^2d\chi\,d\Omega$. Multiplying by $n(z)=n_0a^{-3}$ cancels the expansion factors, equivalently using the comoving volume element directly. Hence

$$
\frac{d^2N}{d\Omega\,dz}=n_0\chi^2\frac{d\chi}{dz}
=\boxed{\frac{4c^3n_0(\sqrt{1+z}-1)^2}{H_0^3(1+z)^{5/2}}.}
$$

This counts every galaxy in the shell per [solid angle](../../../../solid-angle.md), rather than intersections weighted by individual galaxy areas. Near $z=0$ it reduces to $n_0(c/H_0)^3z^2$, as expected for a Euclidean volume shell.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
