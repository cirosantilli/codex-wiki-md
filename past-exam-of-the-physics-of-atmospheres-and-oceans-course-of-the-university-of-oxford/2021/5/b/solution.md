<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $u=U+u'$, $v=v'$, and $\xi=\xi'$, with $U=\bar u$ constant. Discarding products of perturbations in the [vorticity equation](../../../../vorticity-equation.md) gives

$$
(\partial_t+U\partial_x)\xi'+\beta v'=0.
$$

Introduce the [streamfunction](../../../../stream-function.md) convention

$$
u'=-\partial_y\psi',\qquad v'=\partial_x\psi',\qquad \xi'=\nabla_h^2\psi'.
$$

It enforces [incompressibility](../../../../incompressible-flow.md) identically. The linear [partial differential equation](../../../../partial-differential-equation-split.md) is

$$
(\partial_t+U\partial_x)\nabla_h^2\psi'+\beta\partial_x\psi'=0.
$$

For the [plane wave](../../../../plane-wave.md) $\psi'=\operatorname{Re}\{\widehat\psi\exp[i(kx+ly-\omega t)]\}$, put $K^2=k^2+l^2>0$. Substitution yields

$$
i(\omega-Uk)K^2\widehat\psi+i\beta k\widehat\psi=0,\qquad
\boxed{\omega=Uk-\frac{\beta k}{k^2+l^2}.}
$$

The first term is the [Doppler shift](../../../../doppler-effect.md) by the background flow; the second is the intrinsic [Rossby wave](../../../../rossby-wave.md) [frequency](../../../../frequency.md). The source's convention $\omega\geq0$ selects representatives of real waves, rather than making this expression nonnegative for arbitrary $k,l$. For $U=0$ and $\beta>0$, nonzero positive [frequency](../../../../frequency.md) requires $k<0$; the conjugate mode has opposite signs of $k,l,\omega$ and describes the same real field.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
