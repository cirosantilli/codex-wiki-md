<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Freeze a uniform state with $0<\alpha<1$, $\rho_i>0$, and seek a finite [characteristic speed](../../../../characteristic-speed.md) $c$. Denote its perturbation amplitudes by $a,v_1,v_2,\pi$. The two [phase](../../../../phase-waves.md)-mass equations and two momentum equations give

$$
(u_1-c)a+\alpha v_1=0,\qquad-(u_2-c)a+(1-\alpha)v_2=0,
$$



$$
\rho_1(u_1-c)v_1+\pi=0,\qquad\rho_2(u_2-c)v_2+\pi=0.
$$

Eliminating the amplitudes gives

$$
\rho_1(1-\alpha)(u_1-c)^2+\rho_2\alpha(u_2-c)^2=0.
$$

With $s^2=\rho_1(1-\alpha)/(\rho_2\alpha)>0$, factor the quadratic over the complex numbers to obtain

$$
\boxed{c_\pm=\frac{u_2\pm is u_1}{1\pm is}=\frac{u_2+s^2u_1}{1+s^2}\pm i\frac{s(u_1-u_2)}{1+s^2}.}
$$

For nonzero relative [velocity](../../../../velocity.md) the speeds are a nonreal conjugate pair. A [Fourier perturbation](../../../../fourier-mode.md) $e^{ik(x-ct)}$ on the growing branch has magnitude $e^{|k|\,|\operatorname{Im}c|t}$. Arbitrarily short waves therefore grow arbitrarily quickly, preventing a continuous dependence estimate in the usual finite-order [Sobolev norms](../../../../sobolev-norm.md). This generic slip state is [ill-posed](../../../../ill-posed-problem.md) as an [initial value problem](../../../../initial-value-problem.md).

The [pressure](../../../../pressure-split.md) has no independent time-evolution equation; it enforces the incompressible [volume](../../../../volume.md) [constraint](../../../../constraint-mechanics.md), so the request concerns the finite [characteristic speeds](../../../../characteristic-speed.md) rather than a freely propagating [pressure](../../../../pressure-split.md) mode. At $u_1=u_2$ the two speeds coincide and this particular nonreal-speed argument disappears; further degeneracy analysis is needed there, rather than calling coincident real speeds complex. The issue is [complex characteristic speeds of a pressure-coupled two-fluid model](../../../../complex-characteristic-speeds-of-a-pressure-coupled-two-fluid-model.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
