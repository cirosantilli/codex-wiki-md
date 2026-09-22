<h1 id="b/5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For [quasi-steady enzyme kinetics at low substrate saturation](../../../../../quasi-steady-enzyme-kinetics-at-low-substrate-saturation.md), the [quasi-steady-state approximation](../../../../../quasi-steady-state-approximation.md) is controlled here by $\varepsilon=e_0/(s_0+K_m)$, rather than by $e_0/s_0$ alone. Even with $e_0\approx s_0$, taking $K_m\gg s_0$ makes $\varepsilon\ll1$ and $\sigma=s_0/K_m=O(\varepsilon)$.

After the initial fast layer $T=O(\varepsilon)$, the third equation gives

$$
y\sim\frac{\sigma x}{(1+\sigma)(1+\rho)\psi}=O(\varepsilon).
$$

Since $\phi=O(\varepsilon)$, the last equation gives $(e_i)_T=(\phi/\varepsilon)y=O(\varepsilon)$. Starting from $e_i(0)=0$, this implies $e_i=O(\varepsilon)$ on bounded intervals of the slow time. The quasi-steady second equation then gives $x=s+O(\varepsilon)$. In the first equation,

$$
s_T=-s+\frac\rho{1+\rho}s+O(\varepsilon)=-\frac{s}{1+\rho}+O(\varepsilon).
$$

Matching to the initial substrate value $s(0)=1$ therefore yields $\boxed{s(T)\sim e^{-T/(1+\rho)}}$. The relation $x\sim s$ is an outer approximation: it does not replace the initial layer needed to reconcile $x(0)=0$ with $s(0)=1$. Likewise the smallness of accumulated inactivated enzyme has been justified for bounded slow times, not arbitrarily long times.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
