<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A constant shift $\phi\mapsto\phi+\epsilon$ leaves every derivative unchanged, and the density has no undifferentiated $\phi$. Thus it is exactly invariant under this [scalar-field shift symmetry](../../../../scalar-field-shift-symmetry.md). Localize the shift parameter temporarily to $\epsilon(x,t)$:

$$
\delta\mathcal L=\rho\phi_t\epsilon_t+\alpha\phi_x\epsilon_x-\beta\phi_{xx}\epsilon_{xx}.
$$

Integrating the last term by parts once identifies the [Noether current for a constant shift with second derivatives](../../../../noether-current-for-a-constant-shift-with-second-derivatives.md):

$$
\boxed{j^0=\rho\phi_t,\qquad j^x=\alpha\phi_x+\beta\phi_{xxx}.}
$$

The [Euler-Lagrange field equation](../../../../euler-lagrange-field-equation.md) is $\rho\phi_{tt}+\alpha\phi_{xx}+\beta\phi_{xxxx}=0$, precisely the [continuity equation](../../../../continuity-equation.md) $\partial_tj^0+\partial_xj^x=0$. Therefore the conserved quantity, when the endpoint current vanishes or the field has suitable periodic/decaying conditions, is

$$
\boxed{Q=\int\rho\phi_t\,dx,}
$$

the total transverse [momentum](../../../../momentum-split.md). More explicitly $dQ/dt=-[\alpha\phi_x+\beta\phi_{xxx}]_{\rm ends}$. The fixed endpoints introduced later can exert transverse forces and break the global shift symmetry of the boundary problem, so vanishing endpoint current must not be inferred merely from fixed displacement.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
