<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\chi_1(\mathbf x,t)$ equal one in phase one and zero in phase two; its interface value is immaterial for area integrals. In the absence of phase change or interfacial [mass](../../../../mass.md) transfer, the distributional phase [mass conservation](../../../../mass-conservation.md) is $\partial_t(\chi_1\rho)+\nabla\cdot(\chi_1\rho\mathbf u)=0$. For a cross-section $S$ of area $A$, define

$$
\boxed{\alpha=\frac1A\int_S\chi_1\,dA,\qquad
\rho_1=\frac1{A\alpha}\int_S\chi_1\rho\,dA,\qquad
u_1=\frac{\int_S\chi_1\rho u_x\,dA}{A\alpha\rho_1}.}
$$

Here the symbol $u_x$ in the integral denotes the axial velocity component, not a derivative. Integrating through an arbitrary axial slice and using zero normal flux at the rigid pipe wall gives

$$
\boxed{\partial_t(\rho_1\alpha)+\partial_x(\rho_1\alpha u_1)=0.}
$$

The velocity is [mass](../../../../mass.md) weighted, so the averaged [mass flux](../../../../mass-flux.md) factors exactly; an unweighted phase mean would not in general have this property. This is the [cross-section averaged phase mass balance](../../../../cross-section-averaged-phase-mass-balance.md).

For phase two use $\chi_2=1-\chi_1$, [volume fraction](../../../../volume-fraction.md) $1-\alpha$, and

$$
\rho_2=\frac{\int_S\chi_2\rho\,dA}{A(1-\alpha)},\qquad
u_2=\frac{\int_S\chi_2\rho u_x\,dA}{A(1-\alpha)\rho_2}.
$$

Then $\boxed{\partial_t[\rho_2(1-\alpha)]+\partial_x[\rho_2(1-\alpha)u_2]=0}$. Mean quantities in a phase that is absent are unnecessary; the products giving conserved masses and fluxes remain the meaningful variables.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [2](../../2.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
