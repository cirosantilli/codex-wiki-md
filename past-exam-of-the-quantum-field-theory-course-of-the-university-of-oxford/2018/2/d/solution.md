<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The change of field and parameters separates the [Lagrangian density](../../../../lagrangian-density.md) in [Euclidean space](../../../../euclidean-norm.md) into

$$
\begin{aligned}
\mathcal L_{\mathrm{ren}}&=\frac12(\partial\phi)^2+\frac12m^2\phi^2
+\frac{\widetilde\lambda_{2k}}{(2k)!}\phi^{2k},\\
\mathcal L_{\mathrm{ct}}&=\frac12\delta Z(\partial\phi)^2+\frac12\delta m^2\phi^2
+\frac{\delta\lambda_{2k}}{(2k)!}\phi^{2k}.
\end{aligned}
$$

The two-leg [counterterm](../../../../counterterm.md) [interaction vertex](../../../../interaction-vertex.md) is $-(\delta Zp^2+\delta m^2)$, with the overall [momentum conservation](../../../../momentum-conservation.md) delta function understood. With $D_0(p)=1/(p^2+m^2)$, the explicit first-order contribution to the [propagator](../../../../propagator.md) is

$$
\boxed{\delta D_{\mathrm{ct}}(p)
=-\frac{\delta Zp^2+\delta m^2}{(p^2+m^2)^2}.}
$$

The minus sign follows either from expanding $e^{-S_{\mathrm{ct}}}$ or from expanding $(p^2+m^2+\delta Zp^2+\delta m^2)^{-1}$.

For $k=2$, the loop correction is $-\widetilde\lambda_4T_D(m)D_0(p)^2/2$. Its [ultraviolet pole](../../../../ultraviolet-pole.md) from [c](../c.md) is

$$
\delta D_{\mathrm{loop}}\big|_{\mathrm{pole}}
=\frac{g_4m^2}{32\pi^2\epsilon}\,D_0(p)^2,
\qquad \widetilde\lambda_4=\mu^{2\epsilon}g_4.
$$

There is no external $p^2$ dependence in the amputated [tadpole diagram](../../../../tadpole-diagram.md), so no one-loop [wave-function renormalization](../../../../wave-function-renormalization.md) is required. The [minimal subtraction scheme](../../../../minimal-subtraction-scheme.md) therefore gives

$$
\boxed{\delta Z^{(1)}=0,\qquad
\delta m^{2(1)}=\frac{g_4m^2}{32\pi^2\epsilon}.}
$$

Only the pole is subtracted: including $1-\gamma_E+\log4\pi$ would impose a different finite subtraction prescription. The defined $\delta m^2$ is the coefficient in $Zm_0^2=m^2+\delta m^2$, not automatically the difference $m_0^2-m^2$ beyond this order.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
