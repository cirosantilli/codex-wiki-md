<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $x=0$ at chamber A and $x=L$ at chamber B. At [steady state](../../../../../steady-state.md), the [diffusion equation](../../../../../diffusion-equation-split.md) with constant positive [diffusion coefficient](../../../../../diffusion-coefficient.md) gives

$$
0=D\frac{d^2c}{dx^2},\qquad c(x)=A+Bx.
$$

The two [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) give $A=c_0$ and $B=-c_0/L$. Thus

$$
\boxed{c(x)=c_0\left(1-\frac{x}{L}\right),\qquad0\leq x\leq L}.
$$

The concentration [gradient](../../../../../gradient.md) is constant, $dc/dx=-c_0/L$. By [Fick's first law](../../../../../fick-s-first-law.md), the [diffusive flux](../../../../../diffusive-flux.md) is $J=-D\,dc/dx=Dc_0/L$, directed from A towards B. The profile is linear independently of $D$, while the flux and the time needed to approach it depend on $D$.

This result assumes no significant bulk flow, [chemoattractant](../../../../../chemoattractant.md) loss to the walls, degradation or cellular uptake. Experimentally, a uniform-concentration control with matched reservoir concentrations tests for directional [cell migration](../../../../../cell-migration.md) caused by flow or apparatus asymmetry; reversing the reservoir concentrations tests whether the directional response follows the chemical [gradient](../../../../../gradient.md). Keeping both reservoirs well mixed and measuring the concentration profile checks the assumed boundary concentrations and whether uptake has distorted it. These controls distinguish the assumed passive [diffusion](../../../../../diffusion.md) field from other directional cues; the derived profile alone does not establish the mechanism of [chemotaxis](../../../../../chemotaxis.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
