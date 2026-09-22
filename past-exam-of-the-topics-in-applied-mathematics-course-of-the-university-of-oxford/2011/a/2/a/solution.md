<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $J$ be population flux. For any fixed control volume $V\subseteq\Omega$, [mass conservation](../../../../../mass-conservation.md) with local production gives

$$
\frac d{dt}\int_Vu\,dx=-\int_{\partial V}J\cdot\nu\,dS+\int_Vf(u)\,dx.
$$

Assume local, isotropic random dispersal, no imposed advection, and constant [diffusion coefficient](../../../../../diffusion-coefficient.md) $D$. [Fick's first law](../../../../../fick-s-first-law.md) is $J=-D\nabla u$. The [divergence theorem](../../../../../divergence-theorem.md) and arbitrariness of $V$ yield

$$
\boxed{u_t=D\nabla^2u+f(u).}
$$

The coefficient has units length squared per time; $f$ has units population density per time. Smoothness sufficient to pass from the integral balance to the local equation is understood. This is a [reaction-diffusion equation](../../../../../reaction-diffusion-system.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
