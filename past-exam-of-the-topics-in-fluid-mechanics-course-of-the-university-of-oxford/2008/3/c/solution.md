<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For constant [phase](../../../../phase-waves.md) [density](../../../../density.md), let $u_1$ be the intrinsic mean axial speed and define

$$
\boxed{D_1=\frac{\int_\Sigma\chi_1v_x^2\,dA}{A\alpha u_1^2}.}
$$

The profile coefficient measures the momentum [flux](../../../../flux.md) relative to a uniform [velocity](../../../../velocity.md) profile with the same mean. Cauchy-Schwarz gives $D_1\geq1$ where the mean is nonzero, with equality for a uniform [phase](../../../../phase-waves.md) profile. At zero mean it is safer to retain the [second moment](../../../../second-moment.md) itself rather than divide by $u_1^2$.

In the stated common-[pressure](../../../../pressure-split.md), no-extra-force closure, the averaged conservative momentum equation is

$$
\rho_1[\partial_t(\alpha u_1)+\partial_x(\alpha D_1u_1^2)]+\alpha p_x=0.
$$

For constant $D_1$, expand its derivatives and use $\alpha_t+u_1\alpha_x+\alpha(u_1)_x=0$. The terms combine as

$$
\partial_t(\alpha u_1)+\partial_x(\alpha D_1u_1^2)=\alpha(u_1)_t+(2D_1-1)\alpha u_1(u_1)_x+(D_1-1)u_1^2\alpha_x.
$$

Therefore

$$
\boxed{\rho_1\{\alpha(u_1)_t+(2D_1-1)\alpha u_1(u_1)_x+(D_1-1)u_1^2\alpha_x\}+\alpha p_x=0.}
$$

This is the [phase momentum profile coefficient](../../../../phase-momentum-profile-coefficient.md) correction. It accounts for the [second moment](../../../../second-moment.md) of [velocity](../../../../velocity.md), not merely a rescaling of the convective speed. A variable coefficient would also produce $\rho_1\alpha u_1^2(D_1)_x$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
