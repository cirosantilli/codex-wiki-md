<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a [magnetic vector potential](../../../../../../magnetic-vector-potential.md) $\mathbf A$ with $\nabla\times\mathbf A=\mathbf B$, and define the total [magnetic helicity](../../../../../../magnetic-helicity.md) by

$$
\boxed{H_M=\int_D\mathbf A\cdot\mathbf B\,dV.}
$$

The value is unchanged by a single-valued [gauge transformation](../../../../../../gauge-transformation.md) $\mathbf A\mapsto\mathbf A+\nabla\chi$, because

$$
\Delta H_M=\int_D\nabla\cdot(\chi\mathbf B)\,dV=\int_{\partial D}\chi\mathbf B\cdot\mathbf n\,dS=0.
$$

Here both the [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md) and the tangent boundary field are essential. In a multiply connected domain, choose the vector potential by extending the tangent field by zero to all space and fixing its decay there, or fix the equivalent circulation convention. This avoids silently varying the non-gradient harmonic ambiguity of a vector potential on the restricted domain.

The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) permits

$$
\partial_t\mathbf A=\mathbf v\times\mathbf B+\nabla\psi,\qquad \partial_t\mathbf B=\nabla\times(\mathbf v\times\mathbf B).
$$

Differentiating $H_M$ and using [integration by parts](../../../../../../integration-by-parts.md) for [curl](../../../../../../curl.md),

$$
\begin{aligned}
\dot H_M&=\int_D(\mathbf v\times\mathbf B)\cdot\mathbf B\,dV+\int_D\nabla\psi\cdot\mathbf B\,dV+\int_D\mathbf A\cdot\nabla\times(\mathbf v\times\mathbf B)\,dV\\
&=2\int_D(\mathbf v\times\mathbf B)\cdot\mathbf B\,dV+\int_{\partial D}\psi\mathbf B\cdot\mathbf n\,dS+\int_{\partial D}\mathbf n\cdot[(\mathbf v\times\mathbf B)\times\mathbf A],dS=0.
\end{aligned}
$$

The volume product vanishes algebraically, the gauge flux vanishes since $\mathbf B\cdot\mathbf n=0$, and the last boundary term vanishes since $\mathbf v=0$. Thus **magnetic helicity is conserved even though viscosity dissipates mechanical energy**.

Through [magnetic flux freezing](../../../../../../magnetic-flux-freezing.md), [magnetic field lines](../../../../../../magnetic-field-line.md) move with the fluid and retain their linkage during every smooth ideal motion. For two thin closed [flux tubes](../../../../../../flux-tube.md) carrying fluxes $\Phi_1,\Phi_2$, their mutual contribution is $2L\Phi_1\Phi_2$, where $L$ is their [linking number](../../../../../../linking-number.md); self-contributions measure twisting and writhing of the tubes. This explains the topological content of [magnetic helicity](../../../../../../magnetic-helicity.md). Conservation of this one scalar is a consequence of the frozen structure, not a complete description of all that structure.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
