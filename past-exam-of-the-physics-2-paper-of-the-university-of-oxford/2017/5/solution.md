<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

In source-free [vacuum](../../../vacuum.md), [Maxwell's equations](../../../maxwell-equations-split.md) read

$$
\nabla\cdot\mathbf E=0,\quad\nabla\cdot\mathbf B=0,\quad
\nabla\times\mathbf E=-\partial_t\mathbf B,\quad
\nabla\times\mathbf B=\mu_0\epsilon_0\partial_t\mathbf E.
$$

Take the [curl](../../../curl.md) of the third equation and use the [curl of the curl identity](../../../curl-of-the-curl-identity.md) $\nabla\times(\nabla\times\mathbf E)=\nabla(\nabla\cdot\mathbf E)-\nabla^2\mathbf E$. Then

$$
\boxed{\nabla^2\mathbf E=\mu_0\epsilon_0\partial_t^2\mathbf E,\qquad
c=\frac1{\sqrt{\mu_0\epsilon_0}}\simeq2.998\times10^8\,\mathrm{m\,s^{-1}}.}
$$

The prescribed [plane wave](../../../plane-wave.md) travels in the $+z$ direction. Its [polarization](../../../polarization-waves.md) is along $x$, and [Faraday's law](../../../faraday-s-law-of-induction.md) requires $B_y=(k/\omega)E_x$ with $\omega=ck$. The wave's [magnetic flux density](../../../magnetic-field-split.md) is therefore

$$
\boxed{\mathbf B(z,t)=\frac{E_0}{c}\cos(kz-\omega t)\hat{\mathbf y},\qquad
B_0=3.34\times10^{-7}\,\mathrm T.}
$$

The direction is also fixed by $\mathbf E\times\mathbf B$ pointing along the propagation direction. A superposed static uniform [magnetic field](../../../magnetic-field-split.md) is not fixed by the oscillatory [electric field](../../../electric-field-split.md); the expression above is the [magnetic field](../../../magnetic-field-split.md) belonging to the wave itself.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2017](../../2017-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
