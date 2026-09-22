<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the established time-periodic response, take a complex separated solution $v=X(x)e^{i\omega t}$ and set $u=\operatorname{Re}v$. The [diffusion equation](../../../../../diffusion-equation-split.md) gives $X''=(i\omega/\nu)X$. For $\omega>0$, define the penetration depth $\delta=\sqrt{2\nu/\omega}$; the spatial roots are $\pm(1+i)/\delta$. Decay at infinity selects

$$
v(x,t)=U_0e^{-(1+i)x/\delta}e^{i\omega t}.
$$

Its real part is the solution of [Stokes' second problem](../../../../../stokes-second-problem.md):

$$
\boxed{u(x,t)=U_0e^{-x/\delta}\cos(\omega t-x/\delta),\qquad\delta=\sqrt{\frac{2\nu}{\omega}}.}
$$

The velocity amplitude decays exponentially, while the phase lags by $x/\delta$. Direct substitution verifies the [diffusion equation](../../../../../diffusion-equation-split.md), and the two [boundary conditions](../../../../../boundary-condition.md) follow immediately.

**These data select a unique periodic response, but do not specify an arbitrary initial transient.** With no initial velocity supplied, one may add any suitable solution of the homogeneous-boundary diffusion problem. The displayed solution is the usual established oscillatory flow after transients have decayed.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
