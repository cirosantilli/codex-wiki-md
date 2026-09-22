<h1 id="11/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Opening the switch removes the source and $R_1$ but leaves a closed path through the [inductor](../../../../inductor.md) and $R_2$. Set the new time origin at switch-off. [Inductor](../../../../inductor.md) current continuity gives $i_L(0)=V_0/R_1=10\,\mathrm A$. Since the two parallel branches are now isolated, [Kirchhoff's current law](../../../../kirchhoff-node-law.md) gives $I_2=-i_L$, and $L\dot i_L=-R_2i_L$. Thus

$$
i_L(t)=\frac{V_0}{R_1}e^{-R_2t/L},\qquad
\tau_{\rm off}=\frac L{R_2}=7.90\,\mathrm{\mu s}.
$$

All the initially stored [magnetic energy](../../../../magnetic-energy.md) is ultimately converted to [Joule heating](../../../../joule-heating.md) in $R_2$:

$$
\boxed{Q_{2,\rm off}=\frac12L\left(\frac{V_0}{R_1}\right)^2
=3.95\times10^{-2}\,\mathrm J.}
$$

Direct integration of $R_2i_L^2(t)$ gives the same result. The initial shared [voltage](../../../../voltage.md) is $v(0^+)=-R_2i_L(0)=-1000\,\mathrm V$; its reversal drives the return current. The ideal circuit permits this transient [voltage](../../../../voltage.md); real switching would also be limited by stray [capacitance](../../../../capacitance.md), breakdown and other parasitic effects.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [11](../../11.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
