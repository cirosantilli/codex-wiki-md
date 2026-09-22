<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The deterministic [stochastic integral](../../../../../stochastic-integral.md) in the solution is centered Gaussian with variance

$$
v(t)=\int_0^ta(s)^{-2}\sigma(s)^2ds.
$$

Therefore $X(t,x)$ has mean $a(t)x$ and variance

$$
V(t)=a(t)^2v(t)
=\int_0^t e^{2\int_s^t\mu(r)dr}\sigma(s)^2ds.
$$

For $t>0$ this is strictly positive, since $\sigma>0$. Its density at $y$ is

$$
\boxed{\frac1{\sqrt{2\pi V(t)}}
\exp\left[-\frac{(y-a(t)x)^2}{2V(t)}\right].}
$$

The boundedness assumptions on $\sigma$ and its reciprocal in particular ensure nondegeneracy; compact-interval [continuity](../../../../../continuous-function.md) is already sufficient for the displayed finite-time construction.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
