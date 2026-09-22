<h1 id="section-a/a2/returned-polarization">Returned polarization</h1>

↑ **Parent:** [Solution](solution.md)

Use the same fixed laboratory $x,y$ axes for the incident and returning [Jones vectors](../../../../jones-vector.md), with $x$ along the fast axis. Remove a common [phase factor](../../../../phase-factor.md) so that the one-pass [Jones matrix](../../../../jones-matrix.md) is $J=\operatorname{diag}(1,i)$. The reverse pass through this reciprocal plate accumulates the same relative [phase retardation](../../../../phase-retardation.md), not its inverse. The mirror has scalar reflection coefficient $r_m$ in these fixed axes. Therefore

$$
\boxed{\mathbf e_{\rm return}=J(r_mI)J\mathbf e_{\rm in}
=r_m\begin{pmatrix}1&0\\0&-1\end{pmatrix}\mathbf e_{\rm in}.}
$$

The effective retardance is $\pi$: the complete return acts as a [half-wave plate](../../../../half-wave-plate.md). For initial [linear polarization](../../../../linear-polarization.md) at angle $\alpha$ to the fast axis,

$$
\begin{pmatrix}\cos\alpha\\\sin\alpha\end{pmatrix}
\longmapsto
\begin{pmatrix}\cos\alpha\\-\sin\alpha\end{pmatrix},
\qquad \boxed{\alpha_{\rm return}=-\alpha\pmod\pi.}
$$

In particular, the $45^\circ$ input used for linear-to-circular conversion returns in [linear polarization](../../../../linear-polarization.md) perpendicular to its original line: $(1,1)/\sqrt2\mapsto(1,-1)/\sqrt2$. An input along either plate axis returns along that same axis.

The wording does not specify the initial [polarization of waves](../../../../polarization-waves.md). Thus “orthogonal linear return” requires the usual $45^\circ$ linearly polarized input; it is not a universal answer for arbitrary polarized input. The [Jones matrix](../../../../jones-matrix.md) above supplies the general answer. A non-normal metallic reflection may introduce different complex reflection coefficients for the two components and would require additional geometry and optical data. Descriptions of the intermediate [circular polarization](../../../../circular-polarization.md) must also account for the reversed propagation direction when assigning handedness.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [A2](../a2.md)
3. [Section A](../../section-a.md)
4. [2019](../../../2019-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
