<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The free [Euclidean action](../../../../euclidean-action.md) has inverse [propagator](../../../../propagator.md) $D=-m\partial_\tau^2+\kappa$. Therefore the thermal [Green's function](../../../../green-s-function-split.md) obeys

$$
\boxed{(-m\partial_\tau^2+\kappa)G^{(0)}(\tau)=\delta_\beta(\tau),\qquad
G^{(0)}(\tau+\beta)=G^{(0)}(\tau),}
$$

where $\delta_\beta$ is the periodic [Dirac delta function](../../../../dirac-delta-function.md). It is continuous, has continuous first derivative away from its source, and satisfies $G'(0^+)-G'(0^-)=-1/m$. These conditions follow by integrating the differential equation across the source and using the bosonic thermal trace.

For $\Omega=\sqrt{\kappa/m}$, solving the homogeneous equation on $0<\tau<\beta$ and imposing these conditions gives

$$
\boxed{G^{(0)}(\tau)=\frac{\cosh[\Omega(\beta/2-\tau)]}{2m\Omega\sinh(\beta\Omega/2)}\quad(0\le\tau\le\beta).}
$$

In particular $g_0\equiv G^{(0)}(0)=\coth(\beta\Omega/2)/(2m\Omega)$. Equivalently $G^{(0)}=\beta^{-1}\sum_ne^{-i\omega_n\tau}/(m\omega_n^2+\kappa)$ with bosonic [Matsubara frequencies](../../../../matsubara-frequency.md) $\omega_n=2\pi n/\beta$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../e/solution.md)
