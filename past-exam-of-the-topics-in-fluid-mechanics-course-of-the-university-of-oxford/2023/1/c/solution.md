<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $A=2\cot\alpha/3+8\mathrm{Re}/15>0$, maximize the [growth rate](../../../../growth-rate.md) $\sigma(k)=\varepsilon(Ak^2-Sk^4)$ over real [wavenumbers](../../../../wavenumber.md). Its [derivative](../../../../derivative.md) is $2\varepsilon k(A-2Sk^2)$, so

$$
\boxed{|k^*|=\sqrt{\frac A{2S}},\qquad
\sigma^*=\frac{\varepsilon A^2}{4S}.}
$$

The second [derivative](../../../../derivative.md) at either nonzero maximizer is $-4\varepsilon A<0$. If $A\leq0$, there is no positive [growth rate](../../../../growth-rate.md) in this model.

To compare growth with transport, restore dimensions. With $\varepsilon=h_0/L$ and $S=2\gamma/(3\rho gL^2\sin\alpha)$, the maximal dimensional [growth rate](../../../../growth-rate.md) is

$$
\Omega^*=\frac{U_0}{L}\sigma^*
=\frac{3\rho gh_0\sin\alpha\,U_0A^2}{8\gamma}.
$$

The corresponding dimensional [wavenumber](../../../../wavenumber.md) is $k^*/L=\sqrt{3\rho g\sin\alpha\,A/(4\gamma)}$, independent of the arbitrary reference length $L$. Let $d$ be the physical slope length. A disturbance convected at the leading [kinematic wave](../../../../kinematic-wave.md) speed $2U_0$ has [residence time](../../../../residence-time.md) $d/(2U_0)$ and accumulates the growth exponent

$$
N=\frac{\Omega^*d}{2U_0}
=\frac{3\rho gh_0\sin\alpha\,A^2d}{16\gamma}
=\frac32\frac d\ell,
\qquad
\boxed{\ell=\frac{8\gamma}{\rho gh_0\sin\alpha\,A^2}.}
$$

Thus **$d\ll\ell$ implies $N\ll1$**, and the amplitude multiplier $e^N$ remains close to one while the disturbance passes down the slope. This is the requested [convective amplification length](../../../../convective-amplification-length.md) criterion. With the exact coefficients used here, one e-fold of convected growth occurs at $d=2\ell/3$; the stated much-less-than criterion is unaffected by this order-one factor. It is a transport-versus-growth estimate within the [long-wave approximation](../../../../long-wave-approximation.md), rather than a boundary-value stability theorem for every possible inlet and outlet condition.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
