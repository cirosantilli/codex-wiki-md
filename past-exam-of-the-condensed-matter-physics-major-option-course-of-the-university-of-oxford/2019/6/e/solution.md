<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $L$ be the junction length perpendicular to the width and $J_0$ be uniform. Put $\kappa=2\pi\Phi/(W\Phi_0)$. Integrating the local [current-phase relation of a superconducting weak link](../../../../current-phase-relation-of-a-superconducting-weak-link.md) over the junction gives

$$
\begin{aligned}
I_s(\Phi;\varphi_c)&=J_0L\int_{-W/2}^{W/2}\sin(\varphi_c-\kappa z)\,dz\\
&=J_0LW\sin\varphi_c\,\frac{\sin(\kappa W/2)}{\kappa W/2}.
\end{aligned}
$$

The odd-in-$z$ term integrates to zero. At fixed central phase $\varphi_c=\varphi(0)$, define $I(0)=J_0LW\sin\varphi_c$. Then

$$
\boxed{I_s(\Phi)=I(0)\frac{\sin(\pi\Phi/\Phi_0)}{\pi\Phi/\Phi_0}.}
$$

The value at zero flux is the continuous limit, and zeros occur at nonzero integer multiples of $\Phi_0$. This signed formula is the source's expression for a fixed phase. If the measured quantity is the maximum sustainable current, maximize over the central phase instead:

$$
\boxed{I_c(\Phi)=J_0LW\left|\frac{\sin(\pi\Phi/\Phi_0)}{\pi\Phi/\Phi_0}\right|.}
$$

For example, at $\Phi=3\Phi_0/2$ the signed coefficient is $-2/(3\pi)$, whereas the critical current is positive. The absolute-value envelope is the [Fraunhofer pattern of a Josephson junction](../../../../fraunhofer-pattern-of-a-josephson-junction.md), shown in the right panel of the original tunnelling figure. Its simple form relies on uniform $J_0$ and the linear phase profile; it is not the two-junction cosine pattern of a [DC SQUID](../../../../dc-squid.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
