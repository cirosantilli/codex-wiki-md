<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The integrated [stochastic differential equation](../../../../stochastic-differential-equation.md) reads

$$
Y(t):=y(t)-y(0)=\int_0^t\eta(s)\,ds.
$$

The [Gaussian white noise](../../../../gaussian-white-noise.md) has zero [expected value](../../../../expected-value-split.md), so

$$
\boxed{\langle y(t)-y(0)\rangle=0.}
$$

Its [Dirac delta](../../../../dirac-delta-function.md) [covariance](../../../../covariance.md) gives

$$
\begin{aligned}
\langle Y(t)^2\rangle
&=\int_0^t\!ds\int_0^t\!ds'\,\langle\eta(s)\eta(s')\rangle\\
&=\Gamma\int_0^t\!ds\int_0^t\!ds'\,\delta(s-s')
=\Gamma t.
\end{aligned}
$$

Thus $\boxed{\langle[y(t)-y(0)]^2\rangle=\Gamma t}$, which is also the [variance](../../../../variance-split.md) because the displacement has zero [expected value](../../../../expected-value-split.md). More generally its [covariance](../../../../covariance.md) is $\langle Y(s)Y(t)\rangle=\Gamma\min(s,t)$. Equivalently $Y(t)=\sqrt\Gamma\,W_t$ for standard [Brownian motion](../../../../brownian-motion-split.md), and the [diffusion coefficient](../../../../diffusion-coefficient.md) is $D=\Gamma/2$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the field theories and collective phenomena in condensed matter course of the University of Oxford](../../../split.md)
5. [Field theories and collective phenomena in condensed matter course of the University of Oxford](../../../../field-theories-and-collective-phenomena-in-condensed-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
