<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because [optical dispersion](../../../../dispersion-optics.md) makes the [refractive index](../../../../refractive-index.md) depend on [wavelength](../../../../wavelength.md), no single [angle of incidence](../../../../angle-of-incidence.md) makes every component of white [light](../../../../light.md) travel parallel to the base. Choose the supplied central visible [wavelength](../../../../wavelength.md) $535\,\mathrm{nm}$, with $n_0=1.86$, as the design component. [Snell's law](../../../../snell-s-law.md) gives

$$
\boxed{i_0=\arcsin[1.86\sin(27.5^\circ)]=59.188^\circ,\qquad
\delta_0=2i_0-55^\circ=63.376^\circ.}
$$

Keep this [angle of incidence](../../../../angle-of-incidence.md) fixed for all colours. The other components have

$$
r_1(n)=\arcsin\frac{\sin i_0}{n},\qquad
r_2(n)=A-r_1(n),\qquad
e(n)=\arcsin[n\sin r_2(n)],\qquad
\delta(n)=i_0+e(n)-A.
$$

Substitution gives

$$
\begin{array}{c|c|c|c}
\lambda\ (\mathrm{nm})&n&r_1&e\\\hline
370&1.94&26.277^\circ&68.800^\circ\\
535&1.86&27.500^\circ&59.188^\circ\\
700&1.83&27.990^\circ&56.210^\circ
\end{array}
$$

All three emerge: the largest value of $n\sin r_2$ is about $0.9323<1$. The angular spread between the extreme supplied [wavelengths](../../../../wavelength.md) is

$$
\boxed{\Delta\theta=e(1.94)-e(1.83)=12.590^\circ\simeq0.21973\,\mathrm{rad}.}
$$

The respective deviations are $72.988^\circ$, $63.376^\circ$ and $60.398^\circ$. Applying the symmetric formula independently to the two extreme [refractive indices](../../../../refractive-index.md) would instead give $72.221^\circ-60.344^\circ=11.877^\circ$; that compares differently oriented [optical prisms](../../../../prism-optics.md), not the emerging components of one fixed white-light beam. It can be a rough approximation but misses the stated fixed-incidence geometry. The supplied $370\,\mathrm{nm}$ value is near [ultraviolet](../../../../ultraviolet.md), so the computed spread refers to the entire supplied band, not a universally defined visible-white spectrum.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
