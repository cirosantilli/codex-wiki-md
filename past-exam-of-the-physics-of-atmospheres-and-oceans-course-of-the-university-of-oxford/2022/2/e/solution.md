<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $a=0,\frac12,1,\frac32,2,\ldots$, put $n=2a=0,1,2,3,4,\ldots$. Repeated [integration by parts](../../../../integration-by-parts.md) gives $\Gamma(n+1)=n!$. The hemispheric thick-limit results are

$$
\begin{array}{c|ccccc}
a&0&1/2&1&3/2&2\\ \hline
F/(\sigma T_s^4)&1&2/(3\tau_0)&1/\tau_0^2&12/(5\tau_0^3)&8/\tau_0^4\\
T_s/T_0&1&(3\tau_0/2)^{1/4}&\tau_0^{1/2}&(5\tau_0^3/12)^{1/4}&(\tau_0^4/8)^{1/4}
\end{array}
$$

The second row assumes fixed surface [temperature](../../../../temperature-split.md); the third assumes fixed absorbed [radiant flux](../../../../radiant-flux.md). In the vertical-ray approximation the first of these rows becomes $1,1/\tau_0,2/\tau_0^2,6/\tau_0^3,24/\tau_0^4$, and the surface [temperature](../../../../temperature-split.md) factors are the inverse fourth roots.

Thus increasing $a$ makes the [atmosphere](../../../../atmosphere.md) colder at every fixed $0<p<p_s$, decreases outgoing [radiation](../../../../radiation.md) at fixed $T_s$, and requires a warmer surface at fixed absorbed [radiant flux](../../../../radiant-flux.md). The case $a=0$ is isothermal and gives $F=\sigma T_s^4$ exactly, including finite [optical depth](../../../../optical-depth.md).

There is an essential approximation limit. The extension of the [integral](../../../../integral-split.md) to infinity is valid for fixed $a$ as $\tau_0\to\infty$, and is not uniform for arbitrarily large $a$ at fixed $\tau_0$. The vertical integrand peaks at $t=2a$, so one needs that peak well above the surface in [optical depth](../../../../optical-depth.md), with a negligible tail beyond $\tau_0$. For example, at $\tau_0=10$ the thick formula predicts $F/(\sigma T_s^4)=20!/(11\,10^{20})\simeq0.00221$ for $a=10$ but approximately $0.04773$ for $a=12$. This artificial increase contradicts the exact monotonicity: in the finite-[optical depth](../../../../optical-depth.md) expression every atmospheric emission factor $(t/\tau_0)^{2a}$ decreases with $a$. At fixed finite $\tau_0$, the exact limiting outgoing [radiant flux](../../../../radiant-flux.md) is the transmitted surface term $2\sigma T_s^4E_3(\tau_0)$, rather than factorial divergence.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
